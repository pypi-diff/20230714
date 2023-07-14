# Comparing `tmp/RobertCommonDriver-0.1.44.tar.gz` & `tmp/RobertCommonDriver-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.44.tar", last modified: Fri Jul 14 07:10:12 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.45.tar", last modified: Fri Jul 14 14:45:45 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.44.tar` & `RobertCommonDriver-0.1.45.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.501853 RobertCommonDriver-0.1.44/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.44/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.44/MANIFEST.in
--rw-rw-rw-   0        0        0      850 2023-07-14 07:10:12.495380 RobertCommonDriver-0.1.44/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.44/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.408750 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0      850 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      212 2023-06-30 06:01:07.000000 RobertCommonDriver-0.1.44/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.410258 RobertCommonDriver-0.1.44/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.44/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.411262 RobertCommonDriver-0.1.44/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.420267 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.444962 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    68933 2023-06-26 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    78652 2023-07-14 06:41:38.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-07-14 07:10:12.501853 RobertCommonDriver-0.1.44/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-07-14 06:58:15.000000 RobertCommonDriver-0.1.44/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.445970 RobertCommonDriver-0.1.44/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.44/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.446967 RobertCommonDriver-0.1.44/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.44/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.461504 RobertCommonDriver-0.1.44/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.493384 RobertCommonDriver-0.1.44/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     5493 2023-07-14 06:57:36.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.797523 RobertCommonDriver-0.1.45/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.45/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.45/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2023-07-14 14:45:45.797523 RobertCommonDriver-0.1.45/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.45/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.709403 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-14 14:45:45.000000 RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      212 2023-06-30 06:01:07.000000 RobertCommonDriver-0.1.45/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.710404 RobertCommonDriver-0.1.45/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.45/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.711404 RobertCommonDriver-0.1.45/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.729010 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.754472 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    68933 2023-06-26 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    78954 2023-07-14 14:41:30.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 14:45:45.797523 RobertCommonDriver-0.1.45/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-07-14 14:42:19.000000 RobertCommonDriver-0.1.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.755471 RobertCommonDriver-0.1.45/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.45/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.756472 RobertCommonDriver-0.1.45/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.45/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.771788 RobertCommonDriver-0.1.45/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:45:45.795523 RobertCommonDriver-0.1.45/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     5502 2023-07-14 12:58:58.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.44/LICENSE` & `RobertCommonDriver-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/PKG-INFO` & `RobertCommonDriver-0.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.44
+Version: 0.1.45
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.44
+Version: 0.1.45
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.45/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .base import IOTBaseCommon, IOTDriver
 
 
 if platform_system().lower() == 'windows':
     import pywintypes
     import win32com.client
 
-    from pythoncom import (CoInitializeEx, CoUninitialize,  COINIT_MULTITHREADED, PumpWaitingMessages, com_error, GetScodeString, Missing)
+    from pythoncom import (CoInitialize, CoInitializeEx, CoUninitialize,  COINIT_MULTITHREADED, PumpWaitingMessages, com_error, GetScodeString, Missing)
 
     sys.coinit_flags = 0  # pythoncom.COINIT_MULTITHREADED == 0
     pywintypes.datetime = pywintypes.TimeType
     win32com.client.gencache.is_readonly = False    # Allow gencache to create the cached wrapper objects
     win32com.client.gencache.Rebuild(verbose=0)  # Under p2exe the call in gencache to __init__() does not happen so we use Rebuild() to force the creation of the gen_py folder
 
 
@@ -650,32 +650,34 @@
             CoUninitialize()
             if self.server_event is not None:
                 self.server_event.close()
             self.disconnect()
 
         def initialize_client(self, opc_class):
             try:
-                CoInitializeEx(COINIT_MULTITHREADED)
+                CoInitialize()
                 self.opc_client = win32com.client.gencache.EnsureDispatch(opc_class, 0)
                 self.server_event = win32com.client.WithEvents(self.opc_client, OPCDA.ServerEvents)
                 self.server_event.set_client(self)
-            except com_error as err:
-                CoUninitialize()
-                self.opc_error = err
+            except (Exception, com_error) as err:
+                self.opc_error = Exception(err.__str__())
                 raise self.opc_error
 
-        def connect(self, server: Optional[str] = None, host: str = 'localhost'):
-            self.host = host
+        def connect(self, server: Optional[str] = None, host: Optional[str] = 'localhost'):
+            self.host = host if host is not None else 'localhost'
             self.server = server
 
             if self.opc_client is None:
                 raise self.opc_error
 
             if self.opc_connected is False:
-                self.opc_client.Connect(self.server, self.host)
+                try:
+                    self.opc_client.Connect(self.server, self.host)
+                except (Exception, com_error) as e:
+                    raise Exception(f"connect fail({self.get_error(e)})")
                 self.opc_connected = True
             return self.opc_connected
 
         def disconnect(self):
             if self.is_connected() is True:
                 try:
                     self.opc_client.Disconnect()
@@ -696,15 +698,15 @@
         def get_opc_servers(self, opc_host):
             return self.opc_client.GetOPCServers(opc_host)
 
         def get_available_properties(self, tag):
             try:
                 return list(self.opc_client.QueryAvailableProperties(tag))
             except com_error as err:
-                raise err
+                raise Exception(f"properties fail({err.__str__()})")
 
         def get_tag_properties(self, tags: list, id: Optional[Union[str, list]] = None):
             """此方法返回标记的Properties。如果您想从服务器读取许多标记，建议只读取所需的属性ID。测试表明，这种方法非常缓慢，并导致一些服务器崩溃。"""
             try:
                 tags, single_tag, valid = OPCDA.OPCCommon.type_check(tags)
                 descriptions = []
                 property_id = []
@@ -792,15 +794,15 @@
                 try:
                     browser = self.opc_client.CreateBrowser()
                 except com_error as e:
                     raise Exception(f"no browser")
 
                 paths, single, valid = OPCDA.OPCCommon.type_check(paths)
                 if not valid:
-                    raise TypeError("paths must be a string or a list of strings")
+                    raise Exception("paths must be a string or a list of strings")
 
                 if len(paths) == 0:
                     paths = ['*']
 
                 nodes = {}
                 node_type = 'Leaf'
                 for path in paths:
@@ -1055,15 +1057,15 @@
         def groups(self) -> list:
             return sorted(list(self.opc_groups.keys()))
 
         def add_group(self, group_name: str, update_rate: int = 1000) -> bool:
             if group_name not in self.opc_groups.keys():
                 try:
                     self.opc_groups[group_name] = self.opc_client.add_group(group_name, update_rate, self.opc_timeout)
-                except com_error as err:
+                except (com_error, Exception) as err:
                     raise Exception(f"add group({group_name}) fail({self.get_error(err)})")
             return True
 
         def remove_group(self, group_name: str):
             group: OPCDA.OPCGroup = self.opc_groups.pop(group_name, None)
             if group is not None:
                 group.exit()
@@ -1240,15 +1242,15 @@
             if self.opc_client is None:
                 opc_classs = self.opc_class.split(';')
                 for i, opc_class in enumerate(opc_classs):
                     try:
                         opc_client = OPCDA.OPCCom(opc_class)
                         self.opc_client = opc_client
                         break
-                    except com_error as err:
+                    except (com_error, Exception) as err:
                         if i == len(opc_classs) - 1:
                             raise Exception(f"get client fail(EnsureDispatch '{opc_class}' fail: {self.get_error(err)})")
             return self.opc_client
 
         def get_error(self, err) -> str:
             hr, msg, exc, arg = err.args
 
@@ -1716,15 +1718,15 @@
                         self.client.connect(info.get('server'), info.get('host'))
                         self.logging(content=f"connect opc({info.get('host')}-{info.get('server')})")
 
                         self.client.add_group(self.configs.get('group'), self.configs.get('update_rate'))
                         self.logging(content=f"add opc group({self.configs.get('group')})")
                 except Exception as e:
                     self._release_client()
-                    raise e
+                    raise Exception(f"connect fail({e.__str__()})")
         return self.client
 
     def _read(self, tags: list):
         try:
             if len(tags) > 0 and self._get_client():
                 chunk_tags = IOTBaseCommon.chunk_list(tags, self.configs.get('read_limit', 100))
                 for chunk_tag in chunk_tags:
```

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.45/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/setup.py` & `RobertCommonDriver-0.1.45/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.44'
+VERSION = '0.1.45'
 DATE = '2023-07-14'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             print(e.__str__())
         time.sleep(4)
 
 
 def test_read_write_service5():
     dict_config = {
         'server': 'Matrikon.OPC.Simulation.1',
-        'host': 'localhost',  # 'host': '192.168.1.40:8810', 192.168.2.131:8810
+        'host': '192.168.1.104:8810',  # 'host': '192.168.1.40:8810', 192.168.2.131:8810
         'enabled': True,
         'group': f'opcda1',  #
         'action': '',
         'read_limit': 50,
         'update_rate': 500
     }
```

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.45/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

