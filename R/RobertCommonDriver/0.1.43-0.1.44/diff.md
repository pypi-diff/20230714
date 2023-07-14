# Comparing `tmp/RobertCommonDriver-0.1.43.tar.gz` & `tmp/RobertCommonDriver-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.43.tar", last modified: Mon Jun 12 02:27:56 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.44.tar", last modified: Fri Jul 14 07:10:12 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.43.tar` & `RobertCommonDriver-0.1.44.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.451947 RobertCommonDriver-0.1.43/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.43/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.43/MANIFEST.in
--rw-rw-rw-   0        0        0      850 2023-06-12 02:27:56.450941 RobertCommonDriver-0.1.43/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.43/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.359636 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0      850 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.43/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.359636 RobertCommonDriver-0.1.43/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.43/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.360610 RobertCommonDriver-0.1.43/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.379169 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38348 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.405483 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    68907 2023-06-12 02:27:00.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566106 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    61893 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-06-12 02:27:56.451947 RobertCommonDriver-0.1.43/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-06-12 02:27:36.000000 RobertCommonDriver-0.1.43/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.407484 RobertCommonDriver-0.1.43/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.43/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.408485 RobertCommonDriver-0.1.43/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.43/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.424264 RobertCommonDriver-0.1.43/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.449940 RobertCommonDriver-0.1.43/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.501853 RobertCommonDriver-0.1.44/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.44/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.44/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2023-07-14 07:10:12.495380 RobertCommonDriver-0.1.44/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.44/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.408750 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-14 07:10:12.000000 RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      212 2023-06-30 06:01:07.000000 RobertCommonDriver-0.1.44/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.410258 RobertCommonDriver-0.1.44/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.44/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.411262 RobertCommonDriver-0.1.44/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.420267 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.444962 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    68933 2023-06-26 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    78652 2023-07-14 06:41:38.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:10:12.501853 RobertCommonDriver-0.1.44/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-07-14 06:58:15.000000 RobertCommonDriver-0.1.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.445970 RobertCommonDriver-0.1.44/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.44/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.446967 RobertCommonDriver-0.1.44/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.44/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.461504 RobertCommonDriver-0.1.44/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:12.493384 RobertCommonDriver-0.1.44/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     5493 2023-07-14 06:57:36.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.43/LICENSE` & `RobertCommonDriver-0.1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/PKG-INFO` & `RobertCommonDriver-0.1.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.43
+Version: 0.1.44
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.43
+Version: 0.1.44
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.44/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/bacnetc.py`

 * *Files 0% similar despite different names*

```diff
@@ -6656,29 +6656,29 @@
 00019ff0: 2869 2025 2038 2929 0d0a 2020 2020 2020  (i % 8))..      
 0001a000: 2020 7265 7475 726e 2072 6574 0d0a 0d0a    return ret....
 0001a010: 2020 2020 6465 6620 436f 6e76 6572 7454      def ConvertT
 0001a020: 6f49 6e74 2873 656c 6629 3a0d 0a20 2020  oInt(self):..   
 0001a030: 2020 2020 2072 6574 7572 6e20 3020 6966       return 0 if
 0001a040: 2073 656c 662e 7661 6c75 6520 6973 204e   self.value is N
 0001a050: 6f6e 6520 656c 7365 2073 7472 7563 742e  one else struct.
-0001a060: 756e 7061 636b 2827 4c27 2c20 7365 6c66  unpack('L', self
+0001a060: 756e 7061 636b 2827 4927 2c20 7365 6c66  unpack('I', self
 0001a070: 2e76 616c 7565 5b3a 345d 2920 2020 2320  .value[:4])   # 
 0001a080: 7265 7475 726e 2076 616c 7565 203d 3d20  return value == 
 0001a090: 6e75 6c6c 203f 2030 203a 2042 6974 436f  null ? 0 : BitCo
 0001a0a0: 6e76 6572 7465 722e 546f 5549 6e74 3332  nverter.ToUInt32
 0001a0b0: 2876 616c 7565 2c20 3029 3b20 2020 7374  (value, 0);   st
 0001a0c0: 7275 6374 2e75 6e70 6163 6b28 2027 6627  ruct.unpack( 'f'
 0001a0d0: 2c20 6275 6666 6572 2029 0d0a 0d0a 2020  , buffer )....  
 0001a0e0: 2020 6465 6620 436f 6e76 6572 7446 726f    def ConvertFro
 0001a0f0: 6d49 6e74 2873 656c 662c 2076 616c 7565  mInt(self, value
 0001a100: 3a20 696e 7429 3a0d 0a20 2020 2020 2020  : int):..       
 0001a110: 2072 6574 203d 2042 4143 6e65 7442 6974   ret = BACnetBit
 0001a120: 5374 7269 6e67 2829 0d0a 2020 2020 2020  String()..      
 0001a130: 2020 7265 742e 7661 6c75 6520 3d20 7374    ret.value = st
-0001a140: 7275 6374 2e70 6163 6b28 274c 272c 2076  ruct.pack('L', v
+0001a140: 7275 6374 2e70 6163 6b28 2749 272c 2076  ruct.pack('I', v
 0001a150: 616c 7565 290d 0a20 2020 2020 2020 2072  alue)..        r
 0001a160: 6574 2e62 6974 735f 7573 6564 203d 2042  et.bits_used = B
 0001a170: 4143 6e65 7454 6f6f 6c2e 696e 745f 746f  ACnetTool.int_to
 0001a180: 5f62 7974 6528 6d61 7468 2e63 6569 6c28  _byte(math.ceil(
 0001a190: 6d61 7468 2e6c 6f67 2876 616c 7565 2c20  math.log(value, 
 0001a1a0: 3229 2929 0d0a 2020 2020 2020 2020 7265  2)))..        re
 0001a1b0: 7475 726e 2072 6574 0d0a 0d0a 636c 6173  turn ret....clas
@@ -20596,15 +20596,15 @@
 00050730: 2034 2920 2f20 3130 290d 0a20 2020 2020   4) / 10)..     
 00050740: 2020 2020 2020 2045 6e74 7269 6573 203d         Entries =
 00050750: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
 00050760: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
 00050770: 302c 204e 6245 6e74 7269 6573 293a 0d0a  0, NbEntries):..
 00050780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00050790: 6164 6420 3d20 7374 7275 6374 2e75 6e70  add = struct.unp
-000507a0: 6163 6b28 274c 272c 2062 7566 6665 725b  ack('L', buffer[
+000507a0: 6163 6b28 2749 272c 2062 7566 6665 725b  ack('I', buffer[
 000507b0: 3420 2b20 6920 2a20 3130 3a38 202b 2069  4 + i * 10:8 + i
 000507c0: 202a 2031 305d 295b 305d 0d0a 2020 2020   * 10])[0]..    
 000507d0: 2020 2020 2020 2020 2020 2020 6275 6666              buff
 000507e0: 6572 5f70 6f72 7420 3d20 6279 7465 6172  er_port = bytear
 000507f0: 7261 7928 3229 0d0a 2020 2020 2020 2020  ray(2)..        
 00050800: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
 00050810: 2072 616e 6765 2832 293a 0d0a 2020 2020   range(2):..    
@@ -20665,15 +20665,15 @@
 00050b80: 7468 202d 2034 2920 2f20 3130 290d 0a20  th - 4) / 10).. 
 00050b90: 2020 2020 2020 2020 2020 2045 6e74 7269             Entri
 00050ba0: 6573 203d 205b 5d0d 0a0d 0a20 2020 2020  es = []....     
 00050bb0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
 00050bc0: 7261 6e67 6528 302c 204e 6245 6e74 7269  range(0, NbEntri
 00050bd0: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
 00050be0: 2020 2020 2020 6164 6420 3d20 7374 7275        add = stru
-00050bf0: 6374 2e75 6e70 6163 6b28 274c 272c 2062  ct.unpack('L', b
+00050bf0: 6374 2e75 6e70 6163 6b28 2749 272c 2062  ct.unpack('I', b
 00050c00: 7566 6665 725b 3420 2b20 6920 2a20 3130  uffer[4 + i * 10
 00050c10: 3a38 202b 2069 202a 2031 305d 295b 305d  :8 + i * 10])[0]
 00050c20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 00050c30: 2020 2020 6275 6666 6572 5f70 6f72 7420      buffer_port 
 00050c40: 3d20 6279 7465 6172 7261 7928 3229 0d0a  = bytearray(2)..
 00050c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00050c60: 666f 7220 6a20 696e 2072 616e 6765 2832  for j in range(2
```

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/modbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,15 +621,15 @@
                 if value_list:
                     return value_list[0]
             elif modbus_point.get_point_data_type == ModbusType.E_MODBUS_HEX:
                 return None
             elif modbus_point.get_point_data_type == ModbusType.E_MODBUS_BITE:
                 return None
             elif modbus_point.get_point_data_type == ModbusType.E_MODBUS_LONG or modbus_point.get_point_data_type == ModbusType.E_MODBUS_LONG_INVERSE:
-                value_list = struct_unpack('HH', struct_pack('l', int(float(str(point_value)))))
+                value_list = struct_unpack('HH', struct_pack('i', int(float(str(point_value)))))
                 if modbus_point.get_point_data_type == ModbusType.E_MODBUS_LONG_INVERSE:
                     value_list = list(value_list)
                     value_list.reverse()
                 return value_list
             elif modbus_point.get_point_data_type == ModbusType.E_MODBUS_FLOAT or modbus_point.get_point_data_type == ModbusType.E_MODBUS_FLOAT_INVERSE:
                 value_list = struct_unpack('HH', struct_pack('f', float(str(point_value))))
                 if modbus_point.get_point_data_type == ModbusType.E_MODBUS_FLOAT_INVERSE:
```

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1651,10 +1651,10 @@
         error = self.results.get('error', {})
         count = self.results.get('count', 0)
         self.update_info(read=count, response=success, cost='{:.2f}'.format((now - start).total_seconds()))
 
         if show_error:
             for err, names in error.items():
                 names = sorted(list(set(names)))
-                self.logging(content=f"get value({len(names)}) fail({err})", level='ERROR', source=','.join(names), pos=self.stack_pos)
+                self.logging(content=f"get value({len(names)}-[{','.join(names)[:100]}]) fail({err})", level='ERROR', source=','.join(names), pos=self.stack_pos)
 
         return success
```

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files 0% similar despite different names*

```diff
@@ -3517,20 +3517,20 @@
             for i in range(ret.bits_used):
                 is_set = value[i] == '1'
                 if is_set:
                     ret.value[int(i / 8)] |= BACnetTool.int_to_byte(1 << (i % 8))
         return ret
 
     def ConvertToInt(self):
-        return 0 if self.value is None else struct.unpack('L', self.value[
+        return 0 if self.value is None else struct.unpack('I', self.value[
                                                                :4])  # return value == null ? 0 : BitConverter.ToUInt32(value, 0);   struct.unpack( 'f', buffer )
 
     def ConvertFromInt(self, value: int):
         ret = BACnetBitString()
-        ret.value = struct.pack('L', value)
+        ret.value = struct.pack('I', value)
         ret.bits_used = BACnetTool.int_to_byte(math.ceil(math.log(value, 2)))
         return ret
 
 
 class BACnetValue:
 
     def __init__(self, tag: BACnetDefine.BACnetApplicationTags = None, value: Any = None):
@@ -8611,15 +8611,15 @@
         elif function == BACnetDefine.BACnetBvlcFunctions.BVLC_READ_BROADCAST_DIST_TABLE:
             self.SendResult(sender, BACnetDefine.BACnetBvlcResults.BVLC_RESULT_READ_BROADCAST_DISTRIBUTION_TABLE_NAK)
             return (0, function, msg_length)
         elif function == BACnetDefine.BACnetBvlcFunctions.BVLC_WRITE_BROADCAST_DISTRIBUTION_TABLE or function == BACnetDefine.BACnetBvlcFunctions.BVLC_READ_BROADCAST_DIST_TABLE_ACK:
             NbEntries = int((msg_length - 4) / 10)
             Entries = []
             for i in range(0, NbEntries):
-                add = struct.unpack('L', buffer[4 + i * 10:8 + i * 10])[0]
+                add = struct.unpack('I', buffer[4 + i * 10:8 + i * 10])[0]
                 buffer_port = bytearray(2)
                 for j in range(2):
                     buffer_port[j] = buffer[8 + i * 10 + 1 - j]
                 port = struct.unpack('I', buffer_port)[0]
 
                 Mask = buffer[10 + i * 10:14 + i * 10]
                 entry = (add, port)
@@ -8633,15 +8633,15 @@
 
             return (0, function, msg_length)
         elif function == BACnetDefine.BACnetBvlcFunctions.BVLC_READ_FOREIGN_DEVICE_TABLE_ACK:
             NbEntries = int((msg_length - 4) / 10)
             Entries = []
 
             for i in range(0, NbEntries):
-                add = struct.unpack('L', buffer[4 + i * 10:8 + i * 10])[0]
+                add = struct.unpack('I', buffer[4 + i * 10:8 + i * 10])[0]
 
                 buffer_port = bytearray(2)
                 for j in range(2):
                     buffer_port[j] = buffer[8 + i * 10 + 1 - j]
                 port = struct.unpack('I', buffer_port)[0]
 
                 for j in range(2):
```

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,682 +1,506 @@
+
 import logging
 import time
+import sys
+import winreg
+import Pyro5.core
 
 from datetime import datetime
-from inspect import stack
-from os import getenv as os_getenv
+from enum import IntEnum
+from os import getenv as os_getenv, path as os_path, getpid, system as os_system
+from psutil import Process
 from platform import system as platform_system
-from Pyro4 import Proxy, expose as pyro4_expose
+from Pyro5.client import Proxy
+from Pyro5.server import Daemon
+from Pyro5.api import expose as pyro5_expose, current_context
 from re import compile as re_compile, IGNORECASE
-from sys import exc_info
+from socket import gethostname, gethostbyname
+from subprocess import Popen
 from typing import Optional, Union, List, Dict, Any
-from threading import Event
+from threading import Event, Thread, Lock
 
 from .base import IOTBaseCommon, IOTDriver
 
 
 if platform_system().lower() == 'windows':
     import pywintypes
-    import pythoncom
     import win32com.client
+
+    from pythoncom import (CoInitializeEx, CoUninitialize,  COINIT_MULTITHREADED, PumpWaitingMessages, com_error, GetScodeString, Missing)
+
+    sys.coinit_flags = 0  # pythoncom.COINIT_MULTITHREADED == 0
     pywintypes.datetime = pywintypes.TimeType
-    vt = dict([(pythoncom.__dict__[vtype], vtype) for vtype in pythoncom.__dict__.keys() if vtype[:2] == "VT"])
     win32com.client.gencache.is_readonly = False    # Allow gencache to create the cached wrapper objects
     win32com.client.gencache.Rebuild(verbose=0)  # Under p2exe the call in gencache to __init__() does not happen so we use Rebuild() to force the creation of the gen_py folder
 
 
 class OPCDA:
 
-    @pyro4_expose
-    class OPCClient:
+    class OPCCommon:
 
-        class GroupEvents:
-            def __init__(self):
-                self.client = None
-
-            def set_client(self, client):
-                self.client = client
-
-            def OnDataChange(self, TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps):
-                if self.client and hasattr(self.client, 'callback_data_change_value'):
-                    self.client.callback_data_change_value('OnDataChange', TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps)
-
-            def OnAsyncReadComplete(self, TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps, Errors):
-                if self.client and hasattr(self.client, 'callback_data_change_value'):
-                    self.client.callback_data_change_value('OnAsyncReadComplete', TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps, Errors)
-
-            def OnAsyncWriteComplete(self, TransactionID, NumItems, ClientHandles, Errors):
-                if self.client and hasattr(self.client, 'callback_data_change_value'):
-                    self.client.callback_data_change_value('OnAsyncWriteComplete', TransactionID, NumItems, ClientHandles, None, None, None, Errors)
+        @staticmethod
+        def get_datetime() -> datetime:
+            return datetime.now()
+
+        @staticmethod
+        def get_datetime_str() -> str:
+            return OPCDA.OPCCommon.get_datetime().strftime('%Y-%m-%d %H:%M:%S')
+
+        @staticmethod
+        def get_timestamp() -> int:
+            return int(time.time())
 
-            def OnAsyncCancelComplete(self, CancelID):
-                # Not working, not in VB either
+        @staticmethod
+        def convert_time(timestamp: float):
+            try:
+                return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(int(timestamp)))
+            except:
                 pass
+            return timestamp
 
-        class ServerEvents:
+        @staticmethod
+        def get_env(name: str, default: Optional[Any] = None):
+            if platform_system().lower() == 'windows':
+                try:
 
-            def __init__(self):
-                self.client = None
+                    value, valuetype = winreg.QueryValueEx(winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, 'SYSTEM\\CurrentControlSet\\Control\Session Manager\Environment', 0, winreg.KEY_READ), name)
+                    return value
+                except:
+                    return default
+            return os_getenv(name, default)
 
-            def set_client(self, client):
-                self.client = client
+        @staticmethod
+        def get_host_ip() -> str:
+            try:
+                ip = gethostbyname(gethostname())
+            except:
+                ip = '0.0.0.0'
+            return ip
 
-            def OnServerShutDown(self, Reason):
-                if self.client and hasattr(self.client, 'callback_shut_down'):
-                    self.client.callback_shut_down(Reason)
+        @staticmethod
+        def get_executable_folder() -> str:
+            """获取当前运行目录"""
+            return os_path.dirname(sys.executable)
+
+        @staticmethod
+        def type_check(tags: Union[list, tuple, str, None]):
+            single = type(tags) not in (list, tuple)
+            tags = tags if tags else []
+            tags = [tags] if single else tags
+            valid = len([t for t in tags if type(t) not in (str, bytes)]) == 0
+            return tags, single, valid
 
-        def __init__(self, opc_class: Optional[str] = None, client_name: Optional[str] = None, **kwargs):
-            pythoncom.CoInitializeEx(pythoncom.COINIT_MULTITHREADED)
+        @staticmethod
+        def wild2regex(content: str):
+            """将Unix通配符glob转换为正则表达式"""
+            return content.replace('.', r'\.').replace('*', '.*').replace('?', '.').replace('!', '^')
 
-            self.kwargs = kwargs
-            self.opc_client = None
-            self.opc_name = ''
-            self.opc_svc_host = None
-            self.opc_svc_port = None
-            self.opc_timeout = kwargs.get('timeout', 10)
+        @staticmethod
+        def tags2trace(tags: list):
+            """将列表标记转换为适合跟踪回调日志的格式化字符串"""
+            arg_str = ''
+            for i, t in enumerate(tags[1:]):
+                if i > 0:
+                    arg_str += ','
+                arg_str += '%s' % t
+            return arg_str
+
+        @staticmethod
+        def exceptional(func, alt_return=None, alt_exceptions=(Exception,), final=None, catch=None):
+            """将异常转换为替代返回值"""
+            def _exceptional(*args, **kwargs):
+                try:
+                    try:
+                        return func(*args, **kwargs)
+                    except alt_exceptions:
+                        return alt_return
+                    except:
+                        if catch:
+                            return catch(sys.exc_info(), lambda: func(*args, **kwargs))
+                        raise
+                finally:
+                    if final:
+                        final()
+            return _exceptional
 
-            self.opc_connected = False
-            self.parent = None
+        @staticmethod
+        def get_quality_string(quality_bits):
+            """Convert OPC quality bits to a descriptive string"""
+            quality = (quality_bits >> 6) & 3
+            return OPCDA.OPCDefine.QUALITY[quality]
 
-            self.opc_class = opc_class if opc_class is not None else os_getenv('OPC_DA_CLASS', 'Matrikon.OPC.Automation;Graybox.OPC.DAWrapper;HSCOPC.Automation;RSI.OPCAutomation;OPC.Automation')
-            self.opc_client_name = client_name if client_name is not None else os_getenv('OPC_DA_CLIENT', 'OPCDA_CLIENT')
+        @staticmethod
+        def split_to_list(values, size: int):
+            if isinstance(values, dict):
+                results = [{}]
+                for k, v in values.items():
+                    if len(results[-1]) >= size:
+                        results.append({k: v})
+                    else:
+                        results[-1][k] = v
+                return results
+            elif isinstance(values, list):
+                return [values[i:i + size] for i in range(0, len(values), size)]
+            return values
 
-            self.data_source = {'cache': 1, 'device': 2}
-            self.opc_status = (0, 'Running', 'Failed', 'NoConfig', 'Suspended', 'Test')
-            self.browser_types = (0, 'Hierarchical', 'Flat')
-            self.access_rights = (0, 'Read', 'Write', 'Read/Write')
-            self.opc_qualitys = ('Bad', 'Uncertain', 'Unknown', 'Good')
+        @staticmethod
+        def get_current_pids() -> str:
+            pids = []
+            pid = getpid()
+            pids.append(str(pid))
+            pids.extend([str(p.pid) for p in Process(pid).children()])
+            return ','.join(pids)
+
+        @staticmethod
+        def get_current_process() -> dict:
+            """获取当前进程信息"""
+            info = {}
+            p = Process(getpid())
+            if p:
+                with p.oneshot():
+                    info['pid'] = p.pid
+                    info['memory'] = p.memory_info().rss / 1024 / 1024
+                    info['threads'] = p.num_threads()
+                    info['status'] = p.status()
+                    info['cpu'] = p.cpu_percent()
+                    info['create'] = OPCDA.OPCCommon.convert_time(p.create_time())
+            return info
+
+        @staticmethod
+        def restart_service(servic_name: str):
+            """重启服务"""
+            bat_path = f"restart.bat"
+            with open(bat_path, 'w') as f:
+                content = f"@echo off\n"  # 关闭bat脚本的输出
+                content = f"{content}echo {OPCDA.OPCCommon.get_datetime_str()}"
+                content = f"{content}choice /t 3 /d y /n >nul\n"  # 延时3秒执行
+                content = f"{content}net stop {servic_name}\n"
+                content = f"{content}net start {servic_name}\n"
+                f.write(content)
+            Popen(bat_path)
+            return True
 
-            ############
-            self.opc_info = {}
+        @staticmethod
+        def register_dll(dll_path: str):
+            dll_path = dll_path.replace('\\', '/')
+            os_system(f"regsvr32 {dll_path}")
+
+        @staticmethod
+        def convert_socket_address(address) -> str:
+            if isinstance(address, tuple) and len(address) > 1:
+                return f"{address[0]}:{address[1]}"
+            return str(address)
+
+    class OPCConfig:
+
+        def __init__(self, service_name: str = 'RobertOPCDAService', service_display: str = 'Robert OPC DA Service', service_desc: str = 'OPC DA Service 20230627 edit by robert'):
+            self.OPC_DA_SERVICE_NAME = service_name
+            self.OPC_DA_SERVICE_DISPLAY_NAME = service_display
+            self.OPC_DA_SERVICE_DESCRIPTION = service_desc
+
+            self.OPC_DA_START = OPCDA.OPCCommon.get_datetime_str()
+            self.OPC_DA_CLASS = OPCDA.OPCCommon.get_env('OPC_DA_CLASS', 'Matrikon.OPC.Automation;Graybox.OPC.DAWrapper;HSCOPC.Automation;RSI.OPCAutomation;OPC.Automation')
+            self.OPC_DA_GATE_HOST = OPCDA.OPCCommon.get_env('OPC_DA_GATE_HOST',  OPCDA.OPCCommon.get_host_ip())
+            self.OPC_DA_GATE_PORT = int(str(OPCDA.OPCCommon.get_env('OPC_DA_GATE_PORT', '8810')))
+            self.OPC_DA_GATE_MODE = OPCDA.OPCCommon.get_env('OPC_DA_GATE_MODE', 'service')
+            self.OPC_DA_GATE_TOKEN_APP = OPCDA.OPCCommon.get_env('OPC_DA_GATE_TOKEN_APP', 'explorer.exe')
+            self.OPC_DA_GATE_TIMEOUT = int(str(OPCDA.OPCCommon.get_env('OPC_DA_GATE_TIMEOUT', '600')))
+            self.OPC_DA_GATE_CONNECT_INTERVAL = int(str(OPCDA.OPCCommon.get_env('OPC_DA_GATE_CONNECT_INTERVAL', '5')))
+            self.OPC_DA_GATE_LIMIT_SIZE = int(str(OPCDA.OPCCommon.get_env('OPC_DA_GATE_LIMIT_SIZE', '25')))
+            self.OPC_DA_GATE_MEMORY_LIMIT = int(str(OPCDA.OPCCommon.get_env('OPC_DA_GATE_MEMORY_LIMIT', '1000')))
+            self.OPC_DA_CLIENT_NAME = OPCDA.OPCCommon.get_env('OPC_DA_CLIENT',  'RobertOPCDA')  # client name
+            self.OPC_DA_GATE_LOG = f"{OPCDA.OPCCommon.get_executable_folder()}/log/service.log".replace('\\', '/')
+
+        def to_json(self):
+            return self.__dict__
+
+    class OPCDefine:
+
+        SOURCE = {'cache': 1, 'device': 2}
+
+        STATUS = (0, 'Running', 'Failed', 'NoConfig', 'Suspended', 'Test')
+
+        BROWSER_TYPE = (0, 'Hierarchical', 'Flat')
+
+        ACCESS_RIGHT = (0, 'Read', 'Write', 'Read/Write')
+
+        QUALITY = ('Bad', 'Uncertain', 'Unknown', 'Good')
+
+    class GroupEvents:
+        """组事件"""
+
+        def __init__(self):
+            self.client = None
+
+        def set_client(self, client):
+            self.client = client
+
+        def OnDataChange(self, TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps):
+            if self.client and hasattr(self.client, 'callback_data_change_value'):
+                self.client.callback_data_change_value('OnDataChange', TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps)
+
+        def OnAsyncReadComplete(self, TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps, Errors):
+            if self.client and hasattr(self.client, 'callback_data_change_value'):
+                self.client.callback_data_change_value('OnAsyncReadComplete', TransactionID, NumItems, ClientHandles, ItemValues, Qualities, TimeStamps, Errors)
+
+        def OnAsyncWriteComplete(self, TransactionID, NumItems, ClientHandles, Errors):
+            if self.client and hasattr(self.client, 'callback_data_change_value'):
+                self.client.callback_data_change_value('OnAsyncWriteComplete', TransactionID, NumItems, ClientHandles, None, None, None, Errors)
+
+        def OnAsyncCancelComplete(self, CancelID):
+            # Not working, not in VB either
+            pass
+
+    class ServerEvents:
+        """服务器事件"""
+
+        def __init__(self):
+            self.client = None
+
+        def set_client(self, client):
+            self.client = client
+
+        def OnServerShutDown(self, Reason):
+            if self.client and hasattr(self.client, 'callback_shut_down'):
+                self.client.callback_shut_down(Reason)
+
+    class VtType(IntEnum):
+        VT_EMPTY = 0
+        VT_NULL = 1
+        VT_I2 = 2
+        VT_I4 = 3
+        VT_R4 = 4
+        VT_R8 = 5
+        VT_CY = 6
+        VT_DATE = 7
+        VT_BSTR = 8
+        VT_DISPATCH = 9
+        VT_ERROR = 10
+        VT_BOOL = 11
+        VT_VARIANT = 12
+        VT_UNKNOWN = 13
+        VT_DECIMAL = 14
+        VT_I1 = 16
+        VT_UI1 = 17
+        VT_UI2 = 18
+        VT_UI4 = 19
+        VT_I8 = 20
+        VT_UI8 = 21
+        VT_INT = 22
+        VT_UINT = 23
+        VT_VOID = 24
+        VT_HRESULT = 25
+        VT_PTR = 26
+        VT_SAFEARRAY = 27
+        VT_CARRAY = 28
+        VT_USERDEFINED = 29
+        VT_LPSTR = 30
+        VT_LPWSTR = 31
+        VT_RECORD = 36
+        VT_FILETIME = 64
+        VT_BLOB = 65
+        VT_STREAM = 66
+        VT_STORAGE = 67
+        VT_STREAMED_OBJECT = 68
+        VT_STORED_OBJECT = 69
+        VT_BLOB_OBJECT = 70
+        VT_CF = 71
+        VT_CLSID = 72
+        VT_TYPEMASK = 4095
+        VT_VECTOR = 4096
+        VT_ARRAY = 8192
+        VT_BYREF = 16384
+        VT_ILLEGAL = 65535
+        VT_RESERVED = 32768
+
+        @classmethod
+        def _missing_(cls, value):
+            return cls.VT_BSTR
+
+    class OPCGroup:
+
+        def __init__(self, name: str, opc_client, update_rate: int, is_subscribed: int = 1, is_active: int = 1, dead_band: int = 0, opc_timeout: float = 5.0):
+            self.name = name
+            self.update_rate = update_rate
+            self.is_subscribed = is_subscribed
+            self.is_active = is_active
+            self.dead_band = dead_band
+            self.opc_client = opc_client
+            self.opc_timeout = opc_timeout
+
+            self.exit_flag = False
+            self.group = None
+            self.group_event = None
+
+            self.tags = {}  # tag: client_handle
+            self.server_handles = {}    # tag: server_handle
+            self.client_handle_values = {}   # client_handle: value
+            self.client_handle = 0
+            self.transaction_id = 0
+            self.transaction_events = {}    # transaction_id: event
 
-            self.opc_groups = {}  # 组
-            self.opc_group_transaction_id = {}  # 订阅ID对应事件
-            self.opc_client_handle = 0
-            self.opc_client_handle_value = {}  # handle: value
-            self.opc_items = {}  # tag client
-            self.opc_logs = []
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            self.group_data_change = OPCDA.OPCCommon.get_timestamp()
 
-            # service
-            self.opc_svc_guid = None
-            self.opc_svc = None
-            self.opc_svc_client = None
-            self.opc_transaction_id = 0
-            self.opc_prev_serv_time = None
+            self.create_group()
 
-            self._update_info(start=IOTBaseCommon.get_timestamp(), pid=IOTBaseCommon.get_pid())
+            Thread(target=self.pump_wait_msg, name="opcda pump", daemon=False).start()
 
         def __del__(self):
             self.exit()
 
         def exit(self):
-            pythoncom.CoUninitialize()
-            self.close(True)
-
-        def set_parent(self, parent):
-            self.parent = parent
-
-        def save_log(self, log_content: str):
-            if isinstance(log_content, str) and len(log_content) > 0:
-                if len(self.logs) >= 500:
-                    self.logs.pop(0)
-                self.logs.append(log_content)
-
-        def logging(self, **kwargs):
-            if self.parent and hasattr(self.parent, 'logging'):
-                self.parent.logging(**kwargs)
-
-        def set_svc_info(self, host: str, port: int, guid: str, client, service):
-            self.opc_svc_guid = guid
-            self.opc_svc = service
-            self.opc_svc_client = client
-            self.opc_svc_host = host
-            self.opc_svc_port = port
-            self._update_info(guid=guid)
-
-        # ####interface###########
-        def get_info(self):
-            return self.opc_info
-
-        def is_connected(self):
-            return self.opc_connected
-
-        def connect(self, name: Optional[str] = None, host: str = 'localhost') -> bool:
-            if self.opc_connected is False:
-                self._update_info(used=time.time(), name=name, host=host)
-                self.logging(content=f"connect({name} - {host})", pos=self.stack_pos)
-
-                self._get_client().Connect(name, host)
-
-                self.opc_name = name
-                self.opc_svc_host = host
-                self.opc_connected = True
-                self._update_info(connected=self.opc_connected)
-
-                self.reset()
-            return self.opc_connected
-
-        def guid(self):
-            return self.opc_svc_guid
-
-        def disconnect(self):
-            self._update_info(used=time.time(), connected=self.opc_connected)
-            self.logging(content=f"disconnect", pos=self.stack_pos)
-            if self.opc_client is not None:
-                self.opc_client.Disconnect()
-
-        @property
-        def stack_pos(self):
-            return f"{IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]})"
-
-        def close(self, del_object: bool = True):
-            self._update_info(used=time.time())
-            self.logging(content=f"close({del_object})", pos=self.stack_pos)
-
-            opc_connected = self.opc_connected
+            self.exit_flag = True
+            if self.group_event:
+                self.group_event.close()
             try:
-                self.opc_connected = False
-                self._remove_groups(self.groups(), opc_connected)
-                if opc_connected is True:
-                    self.disconnect()
-            except pythoncom.com_error as err:
-                self.logging(content=f"close fail({self._get_error(err)})", level='ERROR', pos=self.stack_pos)
-            except Exception as e:
-                self.logging(content=f"close fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
-            finally:
-                # Remove this object from the open gateway service
-                if self.opc_svc and del_object:
-                    self.opc_svc.release_client(self.opc_svc_client)
-                    self.opc_svc_client = None
-
-        def groups(self) -> list:
-            self._update_info(used=time.time())
-            return sorted(list(self.opc_groups.keys()))
-
-        def add_group(self, group_name: str, update_rate: int = 1000) -> bool:
-            if group_name not in self.opc_groups.keys():
-                self._update_info(used=time.time(), group=group_name)
-                self.logging(content=f"add group({group_name})", pos=self.stack_pos)
-                try:
-                    opc_groups = self._get_client().OPCGroups
-                    opc_group = opc_groups.Add(group_name)
-                    opc_group.IsSubscribed = 1
-                    opc_group.IsActive = 1
-                    opc_group.DeadBand = 0
-                    opc_group.UpdateRate = update_rate
-
-                    group_event = win32com.client.WithEvents(opc_group, self.GroupEvents)
-                    group_event.set_client(self)
-
-                    self._update_group_info(group_name, group=opc_group, group_event=group_event)
-                except pythoncom.com_error as err:
-                    raise Exception(f"add group({group_name}) fail({self._get_error(err)})")
-            return True
-
-        def remove_group(self, group_name: str):
-            self._update_info(used=time.time(), group=None)
-            self.logging(content=f"remove group({group_name})", pos=self.stack_pos)
-
-            if self.opc_client is not None:
-                self.opc_client.OPCGroups.Remove(group_name)
-
-        def add_items(self, group_name: str, item_tags: list):
-            self._update_info(used=time.time())
-            if group_name in self.opc_groups.keys():
-                tags, single, valid = self._type_check(item_tags)
-                if valid is False:
-                    raise Exception(f"tags must be a string or a list of strings")
-
-                new_tags = []
-                for item_tag in item_tags:
-                    if self._check_item_exist(group_name, item_tag) is False:
-                        new_tags.append(item_tag)
-
-                valid_tags = []
-                client_handles = []
-                error_msgs = {}
-
-                group_tags = self._get_group_info(group_name, 'tags', {})
-
-                if len(new_tags) > 0:
-                    errors = self._check_items(group_name, new_tags.copy())
-
-                    for i, item_tag in enumerate(new_tags):
-                        if errors[i] == 0:
-                            valid_tags.append(item_tag)
-                            self.opc_client_handle = self.opc_client_handle + 1
-                            group_tags[item_tag] = self.opc_client_handle
-                            client_handles.append(self.opc_client_handle)
-                        else:
-                            error_msgs[item_tag] = self._get_client().GetErrorString(errors[i])
-
-                    self._update_group_info(group_name, tags=group_tags)
-                    self._update_info(tags=len(group_tags))
-
-                    if len(valid_tags) > 0:
-                        self.logging(content=f"add group({group_name}) item({len(valid_tags)})", pos=self.stack_pos)
-                        server_handles, errors = self._add_items(group_name, client_handles.copy(), valid_tags.copy())
-                        if len(server_handles) > 0:
-                            valid_tags_tmp = []
-                            server_handles_tmp = []
-
-                            group_tags_handles = self._get_group_info(group_name, 'tags_handles', {})
-
-                            for i, tag in enumerate(valid_tags):
-                                if errors[i] == 0:
-                                    valid_tags_tmp.append(tag)
-                                    server_handles_tmp.append(server_handles[i])
-                                    group_tags_handles[tag] = server_handles[i]
-                                else:
-                                    error_msgs[tag] = self._get_client().GetErrorString(errors[i])
-
-                            self._update_group_info(group_name, tags_handles=group_tags_handles)
-                            return True if len(valid_tags_tmp) > 0 else False, valid_tags_tmp, error_msgs  # 只要有一个点添加成功即为正确
-                        return False, [], dict.fromkeys(item_tags, 'add item fail')  # 添加点失败
-                    return False, [], error_msgs  # 点都不正确
-                return True, [], {}  # 无需额外添加点
-            return False, [], dict.fromkeys(item_tags, 'group not exist')  # 组不存在
-
-        def remove_items(self, group_name: str, item_tags: list):
-            self._update_info(used=time.time())
-            self.logging(content=f"remove group({group_name}) items({len(item_tags)})", pos=self.stack_pos)
-
-            if group_name in self.opc_groups.keys():
-                tags, single, valid = self._type_check(item_tags)
-                if not valid:
-                    raise Exception(f"tags must be a string or a list of strings")
-
-                new_tags = []
-                for item_tag in item_tags:
-                    if self._check_item_exist(group_name, item_tag) is True:
-                        new_tags.append(item_tag)
-
-                if len(new_tags) > 0:
-                    server_handles = []
-
-                    group_tags_handles = self._get_group_info(group_name, 'tags_handles', {})
-
-                    for item_tag in new_tags:
-                        if item_tag in group_tags_handles.keys():
-                            server_handles.append(group_tags_handles[item_tag])
-
-                    if len(server_handles) > 0:
-                        server_handles.insert(0, 0)
-                        self._remove_items(group_name, server_handles)
-
-                    group_tags = self._get_group_info(group_name, 'tags', {})
-
-                    for item_tag in new_tags:
-                        if item_tag in group_tags_handles.keys():
-                            del group_tags_handles[item_tag]
-                        if item_tag in group_tags.keys():
-                            del group_tags[item_tag]
-
-                    self._update_info(tags=group_tags)
-
-        def get_datetime_str(self) -> str:
-            return datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-
-        def callback_data_change_value(self, action: str, transaction_id: int, item_num: int, client_handles: list, values: list, qualities: list, timestamps: list, errors: Optional[list] = None):
-            if action in ['OnDataChange', 'OnAsyncReadComplete']:
-                now_str = self.get_datetime_str()
-                for i in range(item_num):
-                    error = ''
-                    if errors is not None and i < len(errors) and errors[i] != 0:
-                        error = self._get_client().GetErrorString(errors[i])
-                    self._update_values(client_handles[i], values[i], qualities[i], timestamps[i], error, now_str)
-
-            if transaction_id == 0:
-                self._update_info(data_change=time.time())
-
-            transaction = self.opc_group_transaction_id.get(transaction_id)
-            if transaction is not None:
-                transaction.set()  # 激活事件
-
-        def callback_shut_down(self, reason):
-            self.opc_connected = False
-            content = f"Server Shutdown({reason}) at {self.get_datetime_str()}"
-            self.logging(content=content, level='ERROR', pos=self.stack_pos)
-
-        def sync_read(self, group_name: str, data_source: int, server_handles: dict):
-            self._update_info(used=time.time())
-
-            opc_group = self.opc_groups.get(group_name, {}).get('group')
-            if opc_group is not None:
-                try:
-                    item_tags = list(server_handles.keys())
-                    server_handles_ = list(server_handles.values())
-                    server_handles_.insert(0, 0)
-                    values, errors, qualities, timestamps = opc_group.SyncRead(data_source, len(server_handles_) - 1, server_handles_)
-                    success = self._parse_value(group_name, item_tags, values, errors, qualities, timestamps)
-                    self.logging(content=f"sync read group({group_name}) ({success}/{len(server_handles)})", pos=self.stack_pos)
-                except pythoncom.com_error as err:
-                    raise Exception(f"sync read group({group_name}) fail({self._get_error(err)})")
-            else:
-                raise Exception(f"sync read group({group_name}) fail(not exist)")
-
-        def _get_transaction_id(self) -> int:
-            self.opc_transaction_id = self.opc_transaction_id + 1
-            return self.opc_transaction_id
-
-        def async_read(self, group_name: str, server_handles: dict):
-            self._update_info(used=time.time())
-            self.logging(content=f"async read group({group_name}) {len(server_handles)}", pos=self.stack_pos)
-
-            opc_group = self.opc_groups.get(group_name, {}).get('group')
-            if opc_group is not None:
-                try:
-                    opc_transaction_id = self._get_transaction_id()
-                    self.opc_group_transaction_id[opc_transaction_id] = Event()
-
-                    server_handles_ = list(server_handles.values())
-                    server_handles_.insert(0, 0)
-                    opc_group.AsyncRead(len(server_handles_) - 1, server_handles_, pythoncom.Missing, self.opc_transaction_id)
-                    if not self.opc_group_transaction_id[opc_transaction_id].wait(self.opc_timeout):
-                        raise Exception(f"async read group({group_name}) fail(Timeout)")
-                except pythoncom.com_error as err:
-                    raise Exception(f"async read group({group_name}) fail({self._get_error(err)})")
-                finally:
-                    del self.opc_group_transaction_id[opc_transaction_id]
-            else:
-                raise Exception(f"async read group({group_name}) fail(not exist)")
+                if self.opc_client and self.opc_client.is_connected() is True:
+                    self.opc_client.OPCGroups.Remove(self.name)
+            except:
+                pass
 
-        def async_refresh(self, group_name: str, data_source: int):
-            self._update_info(used=time.time())
-            self.logging(content=f"async refresh group({group_name})", pos=self.stack_pos)
+            self.client_handle = 0
+            self.transaction_id = 0
+            self.tags = {}
+            self.server_handles = {}
+            self.client_handle_values = {}
+            self.transaction_events = {}
+
+        def info(self) -> dict:
+            """组详情"""
+            return {'name': self.name, 'update_rate': self.update_rate, 'size': len(self.tags), 'use': self.group_use, 'data_change': self.group_data_change}
+
+        def create_group(self):
+            """创建组"""
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            try:
+                self.group = self.opc_client.OPCGroups.Add(self.name)
+                self.group.IsSubscribed = self.is_subscribed
+                self.group.IsActive = self.is_active
+                self.group.DeadBand = self.dead_band
+                self.group.UpdateRate = self.update_rate
+                self.group_event = win32com.client.WithEvents(self.group, OPCDA.GroupEvents)
+                self.group_event.set_client(self)
+            except com_error as e:
+                raise Exception(f"create group fail({self.get_error(e)})")
+
+        def valid_items(self, tags: list):
+            """检查tag是否有效"""
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            try:
+                tags.insert(0, 0)
+                return self.group.OPCItems.Validate(len(tags) - 1, tags)
+            except com_error as e:
+                raise Exception(f"valid item fail({self.get_error(e)})")
 
-            opc_group = self.opc_groups.get(group_name, {}).get('group')
-            if opc_group is not None:
-                try:
-                    opc_transaction_id = self._get_transaction_id()
-                    self.opc_group_transaction_id[opc_transaction_id] = Event()
-                    opc_group.AsyncRefresh(data_source, self.opc_transaction_id)
-                    if not self.opc_group_transaction_id[opc_transaction_id].wait(self.opc_timeout):
-                        raise Exception(f"async refresh group({group_name}) fail(Timeout)")
-                except pythoncom.com_error as err:
-                    raise Exception(f"async refresh group({group_name}) fail({self._get_error(err)})")
-                finally:
-                    del self.opc_group_transaction_id[opc_transaction_id]
-            else:
-                raise Exception(f"async refresh group({group_name}) fail(not exist)")
+        def add_items(self, client_handles: list, valid_tags: list):
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            try:
+                client_handles.insert(0, 0)
+                valid_tags.insert(0, 0)
+                return self.group.OPCItems.AddItems(len(client_handles) - 1, valid_tags, client_handles)
+            except com_error as e:
+                raise Exception(f"add items fail({self.get_error(e)})")
 
-        def read(self, group_name: str, item_tags: Optional[list] = None, action: str = '', source: str = 'cache', size: int = 100, interval: float = 0.1) -> dict:
-            self._update_info(used=time.time())
+        def remove_items(self, server_handles: list):
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            try:
+                server_handles.insert(0, 0)
+                return self.group.OPCItems.Remove(len(server_handles) - 1, server_handles)
+            except com_error as e:
+                raise Exception(f"remove items fail({self.get_error(e)})")
 
-            results = {}
-            if self.opc_connected is True:
-                item_tags = [] if item_tags is None else item_tags
-                if len(item_tags) > 0:
-                    result, success, errors = self.add_items(group_name, item_tags)
-                    if len(errors) > 0:
-                        results.update(errors)
-                    if len(success) > 0:
-                        action = 'sync'
+        def sync_read(self, data_source: int, server_handles: dict):
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            try:
+                item_tags = list(server_handles.keys())
+                server_handles_ = list(server_handles.values())
+                server_handles_.insert(0, 0)
+                values, errors, qualities, timestamps = self.group.SyncRead(data_source, len(server_handles_) - 1, server_handles_)
+                _errors = []
+                for error in errors:
+                    if error == 0:
+                        _errors.append((True, ''))
+                    else:
+                        _errors.append((False, self.get_error_string(error)))
+                self.parse_value(item_tags, values, _errors, qualities, timestamps)
+            except com_error as e:
+                raise Exception(f"sync read fail{self.get_error(e)}")
 
-                valid_item_tags = []
-                if len(item_tags) > 0:
-                    for item_tag in item_tags:
-                        if self._check_item_exist(group_name, item_tag) is True:
-                            valid_item_tags.append(item_tag)
-                else:
-                    opc_group_tags = self.opc_groups.get(group_name, {}).get('tags', {})
-                    for item_tag in opc_group_tags.keys():
-                        valid_item_tags.append(item_tag)
-
-                #
-                if action == 'refresh':  # async异步刷新
-                    results.update(self._read(group_name, valid_item_tags, action, source))
-                else:
-                    item_tags_groups = self._split_to_list(valid_item_tags, size)
-                    for item_tags in item_tags_groups:
-                        results.update(self._read(group_name, item_tags, action, source))
-                        time.sleep(interval)
-            else:
-                raise Exception(f"{self.opc_name} not connected")
-            return results
+        def async_read(self, server_handles: dict):
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            try:
+                opc_transaction_id = self.add_transaction()
+                server_handles_ = list(server_handles.values())
+                server_handles_.insert(0, 0)
+                self.group.AsyncRead(len(server_handles_) - 1, server_handles_, Missing, opc_transaction_id)
+                self.wait_transaction(opc_transaction_id, self.opc_timeout)
+            except com_error as e:
+                raise Exception(f"async read fail{self.get_error(e)}")
 
-        def sync_write(self, group_name: str, server_handles: list, item_values: list, item_tags: list):
-            self._update_info(used=time.time())
-            self.logging(content=f"sync write group({group_name}) ({len(server_handles)})", pos=self.stack_pos)
+        def async_refresh(self, data_source: int):
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
+            try:
+                opc_transaction_id = self.add_transaction()
+                self.group.AsyncRefresh(data_source, opc_transaction_id)
+                self.wait_transaction(opc_transaction_id, self.opc_timeout)
+            except com_error as e:
+                raise Exception(f"async refresh fail {self.get_error(e)}")
 
+        def sync_write(self, server_handles: list, item_values: list, item_tags: list) -> dict:
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
             results = {}
             try:
-                opc_group = self.opc_groups.get(group_name, {}).get('group')
-                if opc_group is not None:
-                    try:
-                        server_handles.insert(0, 0)
-                        item_values.insert(0, 0)
-                        errors = opc_group.SyncWrite(len(server_handles) - 1, server_handles, item_values)
-                        for i, item_tag in enumerate(item_tags):
-                            if errors[i] == 0:
-                                results[item_tag] = [True, '']
-                            else:
-                                results[item_tag] = [False, self._get_error(errors[i])]
-                    except pythoncom.com_error as err:
-                        raise Exception(f'sync write group({group_name}) fail({self._get_error(err)})')
-                else:
-                    raise Exception(f"sync write group({group_name}) fail(no group)")
-            except Exception as e:
-                for item_tag in item_tags:
-                    results[item_tag] = [False, e.__str__()]
+                server_handles.insert(0, 0)
+                item_values.insert(0, 0)
+                errors = self.group.SyncWrite(len(server_handles) - 1, server_handles, item_values)
+                for i, item_tag in enumerate(item_tags):
+                    if errors[i] == 0:
+                        results[item_tag] = [True, '']
+                    else:
+                        results[item_tag] = [False, self.get_error_string(errors[i])]
+            except com_error as e:
+                raise Exception(f"sync write fail{self.get_error(e)}")
             return results
 
-        def async_write(self, group_name: str, server_handles: list, item_values: list, item_tags: list):
-            self._update_info(used=time.time())
-            self.logging(content=f"async write group({group_name}) {len(server_handles)}", pos=self.stack_pos)
-
+        def async_write(self, server_handles: list, item_values: list, item_tags: list):
+            self.group_use = OPCDA.OPCCommon.get_timestamp()
             results = {}
             try:
-                opc_group = self.opc_groups.get(group_name, {}).get('group')
-                if opc_group is not None:
-                    try:
-                        server_handles.insert(0, 0)
-                        item_values.insert(0, 0)
-
-                        opc_transaction_id = self._get_transaction_id()
-                        self.opc_group_transaction_id[opc_transaction_id] = Event()
-                        opc_group.AsyncWrite(len(server_handles) - 1, server_handles, item_values, pythoncom.Missing, self.opc_transaction_id)
-                        for item_tag in item_tags:
-                            results[item_tag] = [True, '']
-                        if not self.opc_group_transaction_id[opc_transaction_id].wait(self.opc_timeout):
-                            raise Exception(f"async write group({group_name}) fail(Timeout)")
-                    except pythoncom.com_error as err:
-                        raise Exception(f'async write group({group_name})({self._get_error(err)})')
-                    finally:
-                        del self.opc_group_transaction_id[opc_transaction_id]
-                else:
-                    raise Exception(f"async write group({group_name})(no group)")
-            except Exception as e:
+                server_handles.insert(0, 0)
+                item_values.insert(0, 0)
+                opc_transaction_id = self.add_transaction()
+                self.group.AsyncWrite(len(server_handles) - 1, server_handles, item_values, Missing, opc_transaction_id)
+                result = [True, '']
+                if self.wait_transaction(opc_transaction_id, self.opc_timeout):
+                    result = [False, 'timeout']
                 for item_tag in item_tags:
-                    results[item_tag] = [False, e.__str__()]
+                    results[item_tag] = result
+            except com_error as e:
+                raise Exception(f"async write fail{self.get_error(e)}")
             return results
 
-        def write(self, group_name: str, items_values: dict, action: str = 'sync', size: int = 100, interval: float = 0.1) -> dict:
-            self._update_info(used=time.time())
-
-            results = {}
-            if self.opc_connected is True:
-                if len(items_values) > 0:
-                    result, success, errors = self.add_items(group_name, list(items_values.keys()))
-                    if len(errors) > 0:
-                        for k, v in errors.items():
-                            results[k] = [False, v]
-                    if len(success) > 0:
-                        action = 'sync'
-
-                valid_item_values = {}
-                if len(items_values) > 0:
-                    for item_tag in items_values.keys():
-                        if self._check_item_exist(group_name, item_tag) is True:
-                            valid_item_values[item_tag] = items_values[item_tag]
-
-                #
-                item_tags_values = self._split_to_list(valid_item_values, size)
-                for item_tags_value in item_tags_values:
-                    results.update(self._write(group_name, item_tags_value, action))
-                    time.sleep(interval)
-            else:
-                raise Exception(f"not connected")
-            return results
-
-        def properties(self, tags: list, ids=None):
-            self._update_info(used=time.time())
-            return list(self._properties(tags, ids))
-
-        def list_items(self, paths: str = '*', recursive: bool = False, flat: bool = False, include_type: bool = False):
-            self._update_info(used=time.time())
-            return list(self._list_items(paths, recursive, flat, include_type))
-
-        def servers(self, opc_host='localhost'):
-            self._update_info(used=time.time())
-            try:
-                servers = self._get_client().GetOPCServers(opc_host)
-                servers = [s for s in servers if s is not None]
-                return servers
-            except pythoncom.com_error as err:
-                raise Exception(f"servers: {self._get_error(err)}")
+        def get_error_string(self, error_id: int):
+            return self.opc_client.GetErrorString(error_id)
 
-        def info(self):
-            self._update_info(used=time.time())
-
-            try:
-                info_list = []
-                mode = 'OpenOPC' if self.opc_svc else 'DCOM'
-
-                info_list.append(('Protocol', mode))
-
-                if mode == 'OpenOPC':
-                    info_list.append(('',))
-                    info_list.append(('Gateway Host', f"{self.opc_svc_host}:{self.opc_svc_port}"))
-                    info_list.append(('Gateway Version', '1.4.0'))
-
-                info_list.append(('Class', self.opc_class))
-                info_list.append(('Client Name', self._get_client().ClientName))
-                info_list.append(('OPC Host', self.opc_svc_host))
-                info_list.append(('OPC Server', self._get_client().ServerName))
-                info_list.append(('State', self.opc_status[self._get_client().ServerState]))
-                info_list.append(('Version', f"{self._get_client().MajorVersion}.{self._get_client().MinorVersion} (Build {self._get_client().BuildNumber})"))
-
-                try:
-                    browser = self._get_client().CreateBrowser()
-                    browser_type = self.browser_types[browser.Organization]
-                except:
-                    browser_type = 'Not Supported'
-
-                info_list.append(('Browser', browser_type))
-                info_list.append(('Start Time', str(self._get_client().StartTime)))
-                info_list.append(('Current Time', str(self._get_client().CurrentTime)))
-                info_list.append(('Vendor', self._get_client().VendorInfo))
-                return info_list
-            except pythoncom.com_error as err:
-                raise Exception(f"info: {self._get_error(err)}")
-
-        def ping(self):
-            self._update_info(used=time.time())
-            try:
-                if self.opc_connected is True:
-                    opc_serv_time = self._get_client().CurrentTime
-                    if opc_serv_time == self.opc_prev_serv_time:
-                        return False
-                    else:
-                        self.opc_prev_serv_time = opc_serv_time
-                        return True
-            except pythoncom.com_error:
-                pass
-            return False
-
-        def get_items(self):
-            item_values = {}
-            for client_handle, item in self.opc_client_handle_value.items():
-                item_values[item.get('tag')] = item.get('value')
-            return item_values
-
-        ##########################
-        def reset(self):
-            self.opc_groups = {}
-            self.opc_group_transaction_id = {}  # 订阅ID对应组号
-            self.opc_client_handle = 0
-            self.opc_client_handle_value = {}  # handle: value
-
-        def _update_handle_value(self, client_handle: int, **kwargs):
-            if client_handle not in self.opc_client_handle_value.keys():
-                self.opc_client_handle_value[client_handle] = {}
-            self.opc_client_handle_value[client_handle].update(**kwargs)
-
-        def _exceptional(self, func, alt_return=None, alt_exceptions=(Exception,), final=None, catch=None):
-            def __exceptional(*args, **kwargs):
-                try:
-                    try:
-                        return func(*args, **kwargs)
-                    except alt_exceptions:
-                        return alt_return
-                    except:
-                        if catch:
-                            return catch(exc_info(), lambda: func(*args, **kwargs))
-                        raise
-                finally:
-                    if final:
-                        final()
-
-            return __exceptional
-
-        def _wild2regex(self, content: str):
-            return content.replace('.', r'\.').replace('*', '.*').replace('?', '.').replace('!', '^')
-
-        def _type_check(self, tags: Union[list, tuple, str, None]):
-            if isinstance(tags, list) or isinstance(tags, tuple):
-                single = False
-            elif tags is None:
-                tags = []
-                single = False
-            else:
-                tags = [tags]
-                single = True
-
-            if len([t for t in tags if type(t) not in (str, bytes)]) == 0:
-                valid = True
-            else:
-                valid = False
-            return tags, single, valid
-
-        def _quality_str(self, quality_bits):
-            quality = (quality_bits >> 6) & 3
-            return self.opc_qualitys[quality]
-
-        def _get_client(self):
-            if self.opc_client is None:
-                opc_client = None
-                opc_classs = self.opc_class.split(';')
-                for i, opc_class in enumerate(opc_classs):
-                    try:
-                        opc_client = win32com.client.gencache.EnsureDispatch(opc_class, 0)
-                        server_event = win32com.client.WithEvents(opc_client, self.ServerEvents)
-                        server_event.set_client(self)
-                        self.opc_class = opc_class
-                        break
-                    except pythoncom.com_error as err:
-                        if i == len(opc_classs) - 1:
-                            raise Exception(f"get client fail(EnsureDispatch '{opc_class}' fail: {self._get_error(err)})")
-                self.opc_client = opc_client
-            return self.opc_client
-
-        def _get_error(self, err) -> str:
+        def get_error(self, err) -> str:
             hr, msg, exc, arg = err.args
 
             if exc is None:
                 error_str = str(msg)
             else:
                 scode = exc[5]
                 try:
-                    opc_err_str = str(self._get_client().GetErrorString(scode)).strip('\r\n')
+                    opc_err_str = str(self.opc_client.GetErrorString(scode)).strip('\r\n')
                 except:
                     opc_err_str = None
 
                 try:
-                    com_err_str = str(pythoncom.GetScodeString(scode)).strip('\r\n')
+                    com_err_str = str(GetScodeString(scode)).strip('\r\n')
                 except:
                     com_err_str = None
 
                 if opc_err_str is None and com_err_str is None:
                     error_str = str(scode)
                 elif opc_err_str == com_err_str:
                     error_str = opc_err_str
@@ -684,218 +508,264 @@
                     error_str = com_err_str
                 elif com_err_str is None:
                     error_str = opc_err_str
                 else:
                     error_str = f'{opc_err_str} ({com_err_str})'
             return error_str
 
-        def _update_info(self, **kwargs):
-            self.opc_info.update(kwargs)
+        def check_tag_exist(self, tag: str) -> bool:
+            return tag in self.tags.keys()
 
-        def _remove_groups(self, groups: list, connect_status: bool = True):
-            for group in groups:
-                opc_group = self.opc_groups.get(group)
-                if isinstance(opc_group, dict):
-                    # 删除组
-                    if connect_status is True:
-                        self.remove_group(group)
-
-                    group_event = opc_group.get('group_event')
-                    if group_event is not None:
-                        group_event.close()
+        def add_tag(self, tag: str):
+            self.client_handle = self.client_handle + 1
+            self.tags[tag] = self.client_handle
+            return self.client_handle
+
+        def add_tag_server_handle(self, tag: str, server_handle):
+            self.server_handles[tag] = server_handle
+
+        def get_tag_server_handle(self, tag: str):
+            return self.server_handles.get(tag)
+
+        def get_tag_value(self, tag: str, property: Union[str, list] = 'value'):
+            """获取标签属性"""
+            if isinstance(property, str):
+                 return self.client_handle_values.get(self.tags.get(tag), {}).get(property)
+            elif isinstance(property, list):
+                value = self.client_handle_values.get(self.tags.get(tag))
+                if isinstance(value, dict):
+                    return [value.get(p) for p in property]
+            return None
+
+        def add_transaction(self):
+            if self.transaction_id >= 0xFFFF:
+                self.transaction_id = 0
+            self.transaction_id = self.transaction_id + 1
+            self.transaction_events[self.transaction_id] = Event()
+            return self.transaction_id
+
+        def wait_transaction(self, transaction_id: int, timeout: Union[int, float]):
+            event = self.transaction_events.pop(transaction_id, None)
+            if event:
+                event.wait(timeout)
+
+        def set_transaction(self, transaction_id: int):
+            event = self.transaction_events.pop(transaction_id, None)
+            if event:
+                event.set()
 
-                    opc_group = {}
-                    del self.opc_groups[group]
+        def get_server_handles(self, tags: list) -> list:
+            return [self.server_handles.get(tag) for tag in tags if tag in self.server_handles.keys()]
 
-        def _check_items(self, group_name: str, item_tags: list) -> list:
-            opc_group = self.opc_groups.get(group_name, {}).get('group')
-            if opc_group is not None:
-                opc_items = opc_group.OPCItems
-                item_tags.insert(0, 0)
-                errors = []
-                try:
-                    errors = opc_items.Validate(len(item_tags) - 1, item_tags)
-                except pythoncom.com_error as err:
-                    raise Exception(f"valid group({group_name}) items fail({self._get_error(err)})")
-                return errors
-            raise Exception(f"valid group({group_name}) items fail")
+        def remove_tags(self, tags: list):
+            for tag in tags:
+                self.tags.pop(tag, None)
+                self.server_handles.pop(tag, None)
 
-        def _add_items(self, group_name: str, client_handles: list, valid_tags: list):
-            opc_group = self.opc_groups.get(group_name, {}).get('group')
-            if opc_group is not None:
-                opc_items = opc_group.OPCItems
-                try:
-                    client_handles.insert(0, 0)
-                    valid_tags.insert(0, 0)
-                    return opc_items.AddItems(len(client_handles) - 1, valid_tags, client_handles)
-                except Exception as e:
-                    self.logging(content=f"add group({group_name}) items fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
-            return [], []
+        def parse_value(self, item_tags: list, values: list, errors: list, qualities: list, timestamps: list) -> int:
+            success = 0
+            now_str = OPCDA.OPCCommon.get_datetime_str()
+            for i, item_tag in enumerate(item_tags):
+                client_handle = self.tags.get(item_tag)
+                if client_handle is not None:
+                    if errors[i][0] is True:
+                        success = success + 1
+                    self.update_values(client_handle, value=str(values[i]), quality=OPCDA.OPCCommon.get_quality_string(qualities[i]), time=str(timestamps[i]), error=errors[i][1], update=now_str, transaction_id=-1)
+            return success
 
-        def _check_item_exist(self, group_name: str, item_tag: str):
-            tags = self.opc_groups.get(group_name, {}).get('tags', {})
-            if item_tag in tags.keys():
-                return True
-            return False
+        def update_values(self, client_handle: int, **kwargs):
+            if client_handle not in self.client_handle_values.keys():
+                self.client_handle_values[client_handle] = {}
+            self.client_handle_values[client_handle].update(**kwargs)
 
-        def _remove_items(self, group_name: str, server_handles: list):
-            opc_group = self.opc_groups.get(group_name, {}).get('group')
-            if opc_group is not None:
-                opc_items = opc_group.OPCItems
+        def callback_data_change_value(self, action: str, transaction_id: int, item_num: int, client_handles: list, values: list, qualities: list, timestamps: list, errors: Optional[list] = None):
+            if transaction_id == 0:
+                self.group_data_change = OPCDA.OPCCommon.get_timestamp()
+
+            if action in ['OnDataChange', 'OnAsyncReadComplete']:
+                now_str = OPCDA.OPCCommon.get_datetime_str()
+                for i in range(item_num):
+                    error = ''
+                    if errors is not None and i < len(errors) and errors[i] != 0:
+                        error = self.get_error_string(errors[i])    # TODO
+                    self.update_values(client_handles[i], value=str(values[i]), quality=OPCDA.OPCCommon.get_quality_string(qualities[i]), time=str(timestamps[i]), error=error, update=now_str, transaction_id=transaction_id)
+            self.set_transaction(transaction_id)    # 激活事件
+
+        def pump_wait_msg(self):
+            while self.exit_flag is False:
                 try:
-                    return opc_items.AddItems(len(server_handles) - 1, server_handles)
-                except pythoncom.com_error as err:
-                    raise Exception(f"remove group({group_name}) items fail({self._get_error(err)})")
+                    if self.opc_client and self.opc_client.is_connected() is True and len(self.tags) > 0:
+                        PumpWaitingMessages()
+                        continue
+                except:
+                    pass
+                time.sleep(0.01)
 
-        def _update_values(self, client_handle: int, value, qualitie, timestamp, error, now_str):
-            self._update_handle_value(client_handle, value=[value if type(value) != pywintypes.TimeType else str(value), self._quality_str(qualitie), str(timestamp), error, now_str])
+    class OPCPyro:
+        """OPC Pyro 实例"""
 
-        def _parse_value(self, group_name: str, item_tags: list, values: list, errors: list, qualities: list, timestamps: list) -> int:
-            success = 0
-            opc_group_tags = self.opc_groups.get(group_name, {}).get('tags', {})
-            now_str = self.get_datetime_str()
-            for i, item_tag in enumerate(item_tags):
-                if item_tag in opc_group_tags.keys():
-                    client_handle = opc_group_tags[item_tag]
-                    if errors[i] == 0:
-                        success = success + 1
-                    self._update_values(client_handle, values[i], qualities[i], timestamps[i], self._get_client().GetErrorString(errors[i]) if errors[i] != 0 else '', now_str)
-            return success
+        def __init__(self, client_id: str, client_socket, client):
+            self.pyro_client_id = client_id
+            self.pyro_client_socket = client_socket
+            self.pyro_client = client
+            self.pyro_create_time = OPCDA.OPCCommon.get_timestamp()   # 创建时间
+            logging.info(f"process({OPCDA.OPCCommon.get_current_pids()}): create session({client_id})")
 
-        def _read(self, group_name: str, item_tags: Optional[list] = None, action: str = '', source: str = 'cache') -> dict:
-            results = {}
-            opc_group = self.opc_groups.get(group_name)
-            if isinstance(opc_group, dict):
+        def __del__(self):
+            self.exit('delete')
 
-                opc_group_server_handles = opc_group.get('tags_handles', {})
-                item_tags = [] if item_tags is None else item_tags
-                if action == '':  # 订阅变化数据
+        def exit(self, reason: str = ''):
+            if self.pyro_client:
+                try:
+                    self.pyro_client.close(True)
+                except:
                     pass
-                elif action in ['sync', 'async']:  # sync同步读取
-                    data_source = self.data_source.get(source, 1)
-                    server_handles = {}
-                    for item_tag in item_tags:
-                        if item_tag in opc_group_server_handles.keys():
-                            server_handles[item_tag] = opc_group_server_handles[item_tag]
+                logging.info(f"process({OPCDA.OPCCommon.get_current_pids()}): close session ({self.pyro_client_id})({reason})")
+            self.pyro_client = None
 
-                    if len(server_handles) > 0:
-                        if action == 'sync':
-                            self.sync_read(group_name, data_source, server_handles)
-                        elif action == 'async':
-                            self.async_read(group_name, server_handles)
-
-                elif action == 'refresh':  # async异步读取
-                    data_source = self.data_source.get(source, 1)
-                    self.async_refresh(group_name, data_source)
+        def get_info(self) -> list:
+            return [self.pyro_client_id, self.pyro_create_time, self.pyro_client.use() if self.pyro_client else self.pyro_create_time, self.get_client_socket()]
 
-                # 返回值
-                opc_group_tags = opc_group.get('tags', {})
-                for item_tag in item_tags:
-                    if item_tag in opc_group_tags.keys():
-                        client_handle = opc_group_tags[item_tag]
-                        self._update_handle_value(client_handle, tag=item_tag)
+        def get_client_socket(self):
+            return OPCDA.OPCCommon.convert_socket_address(self.pyro_client_socket.client_sock_addr)
 
-                        if client_handle in self.opc_client_handle_value.keys():
-                            results[item_tag] = self.opc_client_handle_value[client_handle].get('value')
-            return results
+    @pyro5_expose
+    class OPCCom:
 
-        def _split_to_list(self, values, size: int):
-            if isinstance(values, dict):
-                results = [{}]
-                for k, v in values.items():
-                    if len(results[-1]) >= size:
-                        results.append({k: v})
-                    else:
-                        results[-1][k] = v
-                return results
-            elif isinstance(values, list):
-                return [values[i:i + size] for i in range(0, len(values), size)]
-            return values
+        def __init__(self, opc_class: str):
+            self.opc_class = opc_class
+            self.opc_client = None
+            self.server_event = None
+            self.opc_connected = False
+            self.opc_error = None
 
-        def _write(self, group_name: str, items_values: dict, action: str = 'sync'):
-            results = {}
-            opc_group = self.opc_groups.get(group_name)
-            if isinstance(opc_group, dict):
-                opc_group_server_handles = opc_group.get('tags_handles', {})
-
-                if action in ['sync', 'async']:  # sync同步读取
-                    server_handles = []
-                    item_tags = []
-                    values = []
-                    for item_tag in items_values.keys():
-                        if item_tag in opc_group_server_handles.keys():
-                            item_tags.append(item_tag)
-                            server_handles.append(opc_group_server_handles[item_tag])
-                            values.append(items_values[item_tag])
+            self.server: Optional[str] = None
+            self.host: str = 'localhost'
+            self.opc_prev_serv_time = None
+            self.initialize_client(opc_class)
 
-                    if len(server_handles) > 0:
-                        if action == 'sync':
-                            results.update(self.sync_write(group_name, server_handles.copy(), values.copy(), item_tags.copy()))
-                        elif action == 'async':
-                            results.update(self.async_write(group_name, server_handles.copy(), values.copy(), item_tags.copy()))
-            return results
+        def __del__(self):
+            self.exit()
+
+        def exit(self):
+            CoUninitialize()
+            if self.server_event is not None:
+                self.server_event.close()
+            self.disconnect()
+
+        def initialize_client(self, opc_class):
+            try:
+                CoInitializeEx(COINIT_MULTITHREADED)
+                self.opc_client = win32com.client.gencache.EnsureDispatch(opc_class, 0)
+                self.server_event = win32com.client.WithEvents(self.opc_client, OPCDA.ServerEvents)
+                self.server_event.set_client(self)
+            except com_error as err:
+                CoUninitialize()
+                self.opc_error = err
+                raise self.opc_error
+
+        def connect(self, server: Optional[str] = None, host: str = 'localhost'):
+            self.host = host
+            self.server = server
+
+            if self.opc_client is None:
+                raise self.opc_error
 
-        def _properties(self, tags: list, id=None):
+            if self.opc_connected is False:
+                self.opc_client.Connect(self.server, self.host)
+                self.opc_connected = True
+            return self.opc_connected
+
+        def disconnect(self):
+            if self.is_connected() is True:
+                try:
+                    self.opc_client.Disconnect()
+                except:
+                    pass
+            self.opc_connected = False
+            self.opc_client = None
+
+        def add_group(self, group_name: str, update_rate: int, timeout: float, is_subscribed: int = 1, is_active: int = 1, dead_band: int = 0):
+            return OPCDA.OPCGroup(group_name, self.opc_client, update_rate, is_subscribed, is_active, dead_band, timeout)
+
+        def create_browser(self):
+            return self.opc_client.CreateBrowser()
+
+        def server_name(self):
+            return self.opc_client.ServerName
+
+        def get_opc_servers(self, opc_host):
+            return self.opc_client.GetOPCServers(opc_host)
+
+        def get_available_properties(self, tag):
+            try:
+                return list(self.opc_client.QueryAvailableProperties(tag))
+            except com_error as err:
+                raise err
+
+        def get_tag_properties(self, tags: list, id: Optional[Union[str, list]] = None):
+            """此方法返回标记的Properties。如果您想从服务器读取许多标记，建议只读取所需的属性ID。测试表明，这种方法非常缓慢，并导致一些服务器崩溃。"""
             try:
-                tags, single_tag, valid = self._type_check(tags)
+                tags, single_tag, valid = OPCDA.OPCCommon.type_check(tags)
+                descriptions = []
+                property_id = []
+
                 if not valid:
                     raise Exception(f"tags must be a string or a list of strings")
 
                 try:
                     id.remove(0)
                     include_name = True
                 except:
                     include_name = False
 
                 if id is not None:
-                    descriptions = []
-
                     if isinstance(id, list) or isinstance(id, tuple):
                         property_id = list(id)
                         single_property = False
                     else:
                         property_id = [id]
                         single_property = True
 
                     for i in property_id:
                         descriptions.append('Property id %d' % i)
                 else:
                     single_property = False
 
                 for tag in tags:
                     if id is None:
-                        count, property_id, descriptions, datatypes = self._get_client().QueryAvailableProperties(tag)
+                        count, property_id, descriptions, datatypes = self.get_available_properties(tag)
                         tag_properties = list(map(lambda x, y: (x, y), property_id, descriptions))
                         property_id = [p for p, d in tag_properties if p > 0]
                         descriptions = [d for p, d in tag_properties if p > 0]
 
                     property_id.insert(0, 0)
-                    values, errors = self._get_client().GetItemProperties(tag, len(property_id) - 1, property_id)
+                    values, errors = self.opc_client.GetItemProperties(tag, len(property_id) - 1, property_id)
 
                     property_id.pop(0)
                     values = [str(v) if type(v) == pywintypes.TimeType else v for v in values]
 
                     # Replace variant id with type strings
                     try:
                         i = property_id.index(1)
-                        values[i] = vt[values[i]]
+                        values[i] = OPCDA.OPCClient.VtType(values[i]).name
                     except:
                         pass
 
                     # Replace quality bits with quality strings
                     try:
                         i = property_id.index(3)
-                        values[i] = self._quality_str(values[i])
+                        values[i] = OPCDA.OPCCommon.get_quality_string(values[i])
                     except:
                         pass
 
                     # Replace access rights bits with strings
                     try:
                         i = property_id.index(5)
-                        values[i] = self.access_rights[values[i]]
+                        values[i] = OPCDA.OPCDefine.ACCESS_RIGHT[values[i]]
                     except:
                         pass
 
                     if id is not None:
                         if single_property:
                             if single_tag:
                                 tag_properties = values
@@ -910,37 +780,39 @@
                     if include_name:
                         tag_properties.insert(0, (0, tag))
                     if not single_tag:
                         tag_properties = [tuple([tag] + list(p)) for p in tag_properties]
 
                     for p in tag_properties:
                         yield p
+            except com_error as err:
+                raise Exception(f"properties fail({self.get_error(err)})")
 
-            except pythoncom.com_error as err:
-                raise Exception(f"properties fail({self._get_error(err)})")
-
-        def _list_items(self, paths: str = '*', recursive: bool = False, flat: bool = False, include_type: bool = False):
+        def list_items(self, paths: str = '*', recursive: bool = False, flat: bool = False, include_type: bool = False):
             try:
                 try:
-                    browser = self._get_client().CreateBrowser()
-                except:
-                    return
+                    browser = self.opc_client.CreateBrowser()
+                except com_error as e:
+                    raise Exception(f"no browser")
 
-                paths, single, valid = self._type_check(paths)
+                paths, single, valid = OPCDA.OPCCommon.type_check(paths)
                 if not valid:
                     raise TypeError("paths must be a string or a list of strings")
+
                 if len(paths) == 0:
                     paths = ['*']
+
                 nodes = {}
+                node_type = 'Leaf'
                 for path in paths:
                     if flat:
                         browser.MoveToRoot()
                         browser.Filter = ''
                         browser.ShowLeafs(True)
-                        pattern = re_compile('^%s$' % self._wild2regex(path), IGNORECASE)
+                        pattern = re_compile('^%s$' % OPCDA.OPCCommon.wild2regex(path), IGNORECASE)
                         matches = filter(pattern.search, browser)
                         if include_type:
                             matches = [(x, node_type) for x in matches]
                         for node in matches:
                             yield node
                         continue
 
@@ -959,33 +831,33 @@
                         found_filter = False
                         path_postfix = '/'
 
                         for i, p in enumerate(path_list):
                             if found_filter:
                                 path_postfix += p + '/'
                             elif p.find('*') >= 0:
-                                pattern = re_compile('^%s$' % self._wild2regex(p), IGNORECASE)
+                                pattern = re_compile('^%s$' % OPCDA.OPCCommon.wild2regex(p), IGNORECASE)
                                 found_filter = True
                             elif len(p) != 0:
                                 pattern = re_compile('^.*$')
                                 browser.ShowBranches()
 
                                 # Branch node, so move down
                                 if len(browser) > 0:
                                     try:
                                         browser.MoveDown(p)
                                         path_str += p + '/'
                                     except:
                                         if i < len(path_list) - 1:
                                             return
-                                        pattern = re_compile('^%s$' % self._wild2regex(p), IGNORECASE)
+                                        pattern = re_compile('^%s$' % OPCDA.OPCCommon.wild2regex(p), IGNORECASE)
 
                                 else:
                                     p = '.'.join(path_list[i:])
-                                    pattern = re_compile('^%s$' % self._wild2regex(p), IGNORECASE)
+                                    pattern = re_compile('^%s$' % OPCDA.OPCCommon.wild2regex(p), IGNORECASE)
                                     break
 
                         browser.ShowBranches()
 
                         if len(browser) == 0:
                             browser.ShowLeafs(False)
                             lowest_level = True
@@ -996,64 +868,688 @@
 
                         matches = filter(pattern.search, browser)
 
                         if not lowest_level and recursive:
                             queue += [path_str + x + path_postfix for x in matches]
                         else:
                             if lowest_level:
-                                matches = [self._exceptional(browser.GetItemID, x)(x) for x in matches]
+                                matches = [OPCDA.OPCCommon.exceptional(browser.GetItemID, x)(x) for x in matches]
                             if include_type:
                                 matches = [(x, node_type) for x in matches]
                             for node in matches:
-                                if not node in nodes:
+                                if node not in nodes:
                                     yield node
                                 nodes[node] = True
-            except pythoncom.com_error as err:
-                raise Exception(f"list item fail({self._get_error(err)})")
+            except com_error as err:
+                raise Exception(f"list item fail({self.get_error(err)})")
 
-        def _update_group_info(self, name: str, **kwargs):
-            if name not in self.opc_groups.keys():
-                self.opc_groups[name] = {'name': name}
-            self.opc_groups[name].update(**kwargs)
+        def servers(self, opc_host='localhost'):
+            try:
+                servers = self.opc_client.GetOPCServers(opc_host)
+                return [s for s in servers if s is not None]
+            except com_error as err:
+                raise Exception(f"servers: {self.get_error(err)}")
 
-        def _get_group_info(self, name: str, key: str, defaul):
-            return self.opc_groups.get(name, {}).get(key, defaul)
+        def info(self):
+            try:
+                info_list = []
+                info_list.append(('Client Name', self.opc_client.ClientName))
+                info_list.append(('OPC Server', self.opc_client.ServerName))
+                info_list.append(('State', self.opc_status[self.opc_client.ServerState]))
+                info_list.append(('Version', f"{self.opc_client.MajorVersion}.{self.opc_client.MinorVersion} (Build {self.opc_client.BuildNumber})"))
+
+                try:
+                    browser = self.opc_client.CreateBrowser()
+                    browser_type = self.browser_types[browser.Organization]
+                except:
+                    browser_type = 'Not Supported'
+                info_list.append(('Browser', browser_type))
+                info_list.append(('Start Time', str(self.opc_client.StartTime)))
+                info_list.append(('Current Time', str(self.opc_client.CurrentTime)))
+                info_list.append(('Vendor', self.opc_client.VendorInfo))
+                return info_list
+            except com_error as err:
+                raise Exception(f"info: {self._get_error(err)}")
+
+        def ping(self):
+            try:
+                if self.is_connected() is True:
+                    opc_serv_time = self.opc_client.CurrentTime
+                    if opc_serv_time == self.opc_prev_serv_time:
+                        return False
+                    else:
+                        self.opc_prev_serv_time = opc_serv_time
+                        return True
+            except com_error:
+                pass
+            return False
+
+        def get_error_string(self, error_id: int):
+            return self.opc_client.GetErrorString(error_id)
+
+        def get_error(self, err) -> str:
+            hr, msg, exc, arg = err.args
+
+            if exc is None:
+                error_str = str(msg)
+            else:
+                scode = exc[5]
+                try:
+                    opc_err_str = str(self.opc_client.GetErrorString(scode)).strip('\r\n')
+                except:
+                    opc_err_str = None
+
+                try:
+                    com_err_str = str(GetScodeString(scode)).strip('\r\n')
+                except:
+                    com_err_str = None
+
+                if opc_err_str is None and com_err_str is None:
+                    error_str = str(scode)
+                elif opc_err_str == com_err_str:
+                    error_str = opc_err_str
+                elif opc_err_str is None:
+                    error_str = com_err_str
+                elif com_err_str is None:
+                    error_str = opc_err_str
+                else:
+                    error_str = f'{opc_err_str} ({com_err_str})'
+            return error_str
+
+        @staticmethod
+        def get_vt_type(datatype_number: int):
+            return OPCDA.VtType(datatype_number).name
+
+        def is_connected(self):
+            return self.opc_connected
+
+        def callback_shut_down(self, reason):
+            self.opc_connected = False
+
+    @pyro5_expose
+    class OPCClient:
+
+        def __init__(self, opc_class: Optional[str] = None, client_name: Optional[str] = None, **kwargs):
+            self.kwargs = kwargs
+            self.opc_client = None
+            self.opc_name = ''
+            self.opc_timeout = kwargs.get('timeout', 10)
+
+            self.opc_class = opc_class if opc_class is not None else OPCDA.OPCCommon.get_env('OPC_DA_CLASS', 'OPC.Automation')
+            self.opc_client_name = client_name if client_name is not None else OPCDA.OPCCommon.get_env('OPC_DA_CLIENT', 'RobertOPCDA')
+
+            ############
+            self.opc_groups = {}  # 组
+            self.opc_infos = {}
+
+            # service
+            self.opc_svc = None
+            self.opc_svc_client = None
+            self.opc_prev_serv_time = None
+            self.opc_svc_host = None
+            self.opc_svc_port = None
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp())
+
+        def __del__(self):
+            self.exit()
+
+        def exit(self):
+            self.close(True)
+
+        def track_resource(self):
+            """服务监视对象"""
+            current_context.track_resource(self)
+
+        def set_svc_info(self, host: str, port: int, client_id, service: Optional[Any] = None):
+            self.opc_svc_host = host
+            self.opc_svc_port = port
+            self.opc_svc = service
+            self.update_infos(guid=client_id)
+
+        # ####interface###########
+        def update_infos(self, **kwargs):
+            self.opc_infos.update(**kwargs)
+
+        def get_info(self) -> dict:
+            self.opc_infos.update(connected=self.is_connected(), groups=[group.info() for group in self.opc_groups.values()])
+            return self.opc_infos
+
+        def connect(self, name: Optional[str] = None, host: str = 'localhost') -> bool:
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp(), name=name, host=host)
+            try:
+                return self._get_client().connect(name, host)
+            finally:
+                if self.opc_svc:
+                    logging.info(f"process({OPCDA.OPCCommon.get_current_pids()}): connect({self.get_info()})")
+
+        def is_connected(self) -> bool:
+            return self.opc_client and self.opc_client.is_connected()
+
+        def guid(self):
+            return self.get_info().get('guid')
+
+        def use(self):
+            """使用时间"""
+            return self.get_info().get('used')
+
+        def disconnect(self):
+            if self.opc_client is not None:
+                self.opc_client.disconnect()
+            self.opc_client = None
+
+        def close(self, del_object: bool = True):
+            try:
+                if self.opc_svc and self.opc_client:
+                    logging.info(f"process({OPCDA.OPCCommon.get_current_pids()}): close({self.get_info()})")
+                group_names = self.groups()
+                for group_name in group_names:
+                    self.remove_group(group_name)
+                self.disconnect()
+            except (com_error, Exception) as e:
+                pass
+            finally:
+                # Remove this object from the open gateway service
+                if self.opc_svc and del_object:
+                    self.opc_svc.release_client(self.opc_svc_client)
+                    self.opc_svc_client = None
+
+        def groups(self) -> list:
+            return sorted(list(self.opc_groups.keys()))
+
+        def add_group(self, group_name: str, update_rate: int = 1000) -> bool:
+            if group_name not in self.opc_groups.keys():
+                try:
+                    self.opc_groups[group_name] = self.opc_client.add_group(group_name, update_rate, self.opc_timeout)
+                except com_error as err:
+                    raise Exception(f"add group({group_name}) fail({self.get_error(err)})")
+            return True
+
+        def remove_group(self, group_name: str):
+            group: OPCDA.OPCGroup = self.opc_groups.pop(group_name, None)
+            if group is not None:
+                group.exit()
+            return True
+
+        def add_items(self, group, item_tags: list):
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp())
+            if group is not None:
+                tags, single, valid = OPCDA.OPCCommon.type_check(item_tags)
+                if valid is False:
+                    raise Exception(f"tags must be a string or a list of strings")
+
+                new_tags = []
+                for item_tag in item_tags:
+                    if group.check_tag_exist(item_tag) is False:
+                        new_tags.append(item_tag)
+
+                valid_tags = []
+                client_handles = []
+                error_msgs = {}
+
+                if len(new_tags) > 0:
+                    errors = group.valid_items(new_tags.copy())
+
+                    for i, item_tag in enumerate(new_tags):
+                        if errors[i] == 0:
+                            valid_tags.append(item_tag)
+                            opc_client_handle = group.add_tag(item_tag)
+                            client_handles.append(opc_client_handle)
+                        else:
+                            error_msgs[item_tag] = group.get_error_string(errors[i])
+
+                    if len(valid_tags) > 0:
+                        server_handles, errors = group.add_items(client_handles.copy(), valid_tags.copy())
+                        if len(server_handles) > 0:
+                            valid_tags_tmp = []
+                            for i, tag in enumerate(valid_tags):
+                                if errors[i] == 0:
+                                    valid_tags_tmp.append(tag)
+                                    group.add_tag_server_handle(tag, server_handles[i])
+                                else:
+                                    error_msgs[tag] = group.get_error_string(errors[i])
+                            return True if len(valid_tags_tmp) > 0 else False, valid_tags_tmp, error_msgs  # 只要有一个点添加成功即为正确
+                        return False, [], dict.fromkeys(item_tags, 'add item fail')  # 添加点失败
+                    return False, [], error_msgs  # 点都不正确
+                return True, [], {}  # 无需额外添加点
+            return False, [], dict.fromkeys(item_tags, 'group not exist')  # 组不存在
+
+        def remove_items(self, group_name: str, item_tags: list):
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp())
+            opc_group: OPCDA.OPCGroup = self.opc_groups.get(group_name)
+            if opc_group is not None:
+                tags, single, valid = OPCDA.OPCCommon.type_check(item_tags)
+                if not valid:
+                    raise Exception(f"tags must be a string or a list of strings")
+
+                new_tags = []
+                for item_tag in item_tags:
+                    if opc_group.check_tag_exist(item_tag) is True:
+                        new_tags.append(item_tag)
+
+                if len(new_tags) > 0:
+                    server_handles = opc_group.get_server_handles(new_tags)
+
+                    if len(server_handles) > 0:
+                        opc_group.remove_items(server_handles)
+
+                    opc_group.remove_tags(new_tags)
+
+        def read(self, group_name: str, item_tags: Optional[list] = None, action: str = '', source: str = 'cache', size: int = 100, interval: float = 0.1) -> dict:
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp())
+            results = {}
+            if self.is_connected() is True:
+                opc_group: OPCDA.OPCGroup = self.opc_groups.get(group_name)
+                if opc_group is not None:
+                    item_tags = [] if item_tags is None else item_tags
+                    if len(item_tags) > 0:
+                        result, success, errors = self.add_items(opc_group, item_tags)
+                        if len(errors) > 0:
+                            results.update(errors)
+                        if len(success) > 0:
+                            action = 'sync'
+
+                    valid_item_tags = []
+                    if len(item_tags) > 0:
+                        for item_tag in item_tags:
+                            if opc_group.check_tag_exist(item_tag) is True:
+                                valid_item_tags.append(item_tag)
+                    else:
+                        valid_item_tags = list(set(list(opc_group.tags.keys())))
+
+                    #
+                    if action == 'refresh':  # async异步刷新
+                        results.update(self._read(group_name, valid_item_tags, action, source))
+                    else:
+                        item_tags_groups = OPCDA.OPCCommon.split_to_list(valid_item_tags, size)
+                        for item_tags in item_tags_groups:
+                            results.update(self._read(group_name, item_tags, action, source))
+                            time.sleep(interval)
+                else:
+                    raise Exception(f"no group({group_name})")
+            else:
+                raise Exception(f"not connected")
+            return results
+
+        def write(self, group_name: str, items_values: dict, action: str = 'sync', size: int = 100, interval: float = 0.1) -> dict:
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp())
+            results = {}
+            if self.is_connected() is True:
+                opc_group: OPCDA.OPCGroup = self.opc_groups.get(group_name)
+                if opc_group is not None:
+                    if len(items_values) > 0:
+                        result, success, errors = self.add_items(opc_group, list(items_values.keys()))
+                        if len(errors) > 0:
+                            for k, v in errors.items():
+                                results[k] = [False, v]
+                        if len(success) > 0:
+                            action = 'sync'
+
+                    valid_item_values = {}
+                    if len(items_values) > 0:
+                        for item_tag in items_values.keys():
+                            if opc_group.check_tag_exist(item_tag) is True:
+                                valid_item_values[item_tag] = items_values[item_tag]
+
+                    #
+                    item_tags_values = OPCDA.OPCCommon.split_to_list(valid_item_values, size)
+                    for item_tags_value in item_tags_values:
+                        results.update(self._write(group_name, item_tags_value, action))
+                        time.sleep(interval)
+            else:
+                raise Exception(f"not connected")
+            return results
+
+        def properties(self, tags: list, ids=None):
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp())
+            if self.is_connected() is True:
+                return list(self.opc_client.get_tag_properties(tags, ids))
+            else:
+                raise Exception(f"not connected")
+
+        def list_items(self, paths: str = '*', recursive: bool = False, flat: bool = False, include_type: bool = False):
+            self.update_infos(used=OPCDA.OPCCommon.get_timestamp())
+            if self.is_connected() is True:
+                return list(self.opc_client.list_items(paths, recursive, flat, include_type))
+            else:
+                raise Exception(f"not connected")
+
+        def servers(self, opc_host='localhost'):
+            return self._get_client().servers(opc_host)
+
+        def info(self):
+            info_list = []
+            mode = 'OpenOPC' if self.opc_svc else 'DCOM'
+            info_list.append(('Protocol', mode))
+            if mode == 'OpenOPC':
+                info_list.append(('',))
+                info_list.append(('Gateway Host', f"{self.opc_svc_host}:{self.opc_svc_port}"))
+                info_list.append(('Gateway Version', '1.4.0'))
+            info_list.append(('Class', self.opc_class))
+            info_list.append(('OPC Host', self.opc_svc_host))
+            if self._get_client():
+                info_list.extend(self.opc_client.info())
+            return info_list
+
+        def ping(self):
+            if self.is_connected() is True:
+                return self.opc_client.ping()
+            else:
+                return False
+
+        ##########################
+        def _get_client(self):
+            if self.opc_client is None:
+                opc_classs = self.opc_class.split(';')
+                for i, opc_class in enumerate(opc_classs):
+                    try:
+                        opc_client = OPCDA.OPCCom(opc_class)
+                        self.opc_client = opc_client
+                        break
+                    except com_error as err:
+                        if i == len(opc_classs) - 1:
+                            raise Exception(f"get client fail(EnsureDispatch '{opc_class}' fail: {self.get_error(err)})")
+            return self.opc_client
+
+        def get_error(self, err) -> str:
+            hr, msg, exc, arg = err.args
+
+            if exc is None:
+                error_str = str(msg)
+            else:
+                scode = exc[5]
+                try:
+                    opc_err_str = str(self.opc_client.GetErrorString(scode)).strip('\r\n')
+                except:
+                    opc_err_str = None
+
+                try:
+                    com_err_str = str(GetScodeString(scode)).strip('\r\n')
+                except:
+                    com_err_str = None
+
+                if opc_err_str is None and com_err_str is None:
+                    error_str = str(scode)
+                elif opc_err_str == com_err_str:
+                    error_str = opc_err_str
+                elif opc_err_str is None:
+                    error_str = com_err_str
+                elif com_err_str is None:
+                    error_str = opc_err_str
+                else:
+                    error_str = f'{opc_err_str} ({com_err_str})'
+            return error_str
+
+        def _read(self, group_name: str, item_tags: Optional[list] = None, action: str = '', source: str = 'cache') -> dict:
+            results = {}
+            if self.is_connected() is True:
+                opc_group: OPCDA.OPCGroup = self.opc_groups.get(group_name)
+                if opc_group is not None:
+                    item_tags = [] if item_tags is None else item_tags
+                    if action == '':  # 订阅变化数据
+                        pass
+                    elif action in ['sync', 'async']:  # sync同步读取
+                        data_source = OPCDA.OPCDefine.SOURCE.get(source, 1)
+                        server_handles = {}
+                        for item_tag in item_tags:
+                            server_handle = opc_group.get_tag_server_handle(item_tag)
+                            if server_handle is not None:
+                                server_handles[item_tag] = server_handle
+
+                        if len(server_handles) > 0:
+                            if action == 'sync':
+                                opc_group.sync_read(data_source, server_handles)
+                            elif action == 'async':
+                                opc_group.async_read(server_handles)
+                    elif action == 'refresh':  # async异步读取
+                        data_source = OPCDA.OPCDefine.SOURCE.get(source, 1)
+                        opc_group.async_refresh(data_source)
+
+                    # 返回值
+                    for item_tag in item_tags:
+                        value = opc_group.get_tag_value(item_tag, ['value', 'quality', 'time', 'error', 'update'])    # v, status, time, error, update
+                        if value is not None:
+                            results[item_tag] = value
+            return results
+
+        def _write(self, group_name: str, items_values: dict, action: str = 'sync'):
+            results = {}
+            if self.is_connected() is True:
+                opc_group: OPCDA.OPCGroup = self.opc_groups.get(group_name)
+                if opc_group is not None:
+                    if action in ['sync', 'async']:  # sync同步读取
+                        server_handles = []
+                        item_tags = []
+                        values = []
+                        for item_tag in items_values.keys():
+                            server_handle = opc_group.get_tag_server_handle(item_tag)
+                            if server_handle is not None:
+                                item_tags.append(item_tag)
+                                server_handles.append(server_handle)
+                                values.append(items_values[item_tag])
+
+                        if len(server_handles) > 0:
+                            if action == 'sync':
+                                results.update(opc_group.sync_write(server_handles.copy(), values.copy(), item_tags.copy()))
+                            elif action == 'async':
+                                results.update(opc_group.async_write(server_handles.copy(), values.copy(), item_tags.copy()))
+            return results
+
+    @pyro5_expose
+    class OPCServer:
+
+        def __init__(self, opc_config: Optional[Any] = None):
+            self.opc_config: OPCDA.OPCConfig = opc_config   # 配置信息
+            self.clients: dict = {}     # id: OPCPyro
+            self.connections = {}       # 连接： ID
+            self.lock = Lock()
+
+        def client_disconnected(self, connection):
+            """
+                客户端关闭事件
+                注意实际调用时候是另起一个连接，实际上就是两次连接
+            """
+            for guid in [r.guid() for r in connection.tracked_resources]:
+                self.force_close(guid, 'disconnected')
+
+        def get_clients(self) -> list:
+            return [client.get_info() for client_id, client in self.clients.items()]
+
+        def close_all_sessions(self, reason: str = ''):
+            for guid in list(self.clients.keys()):
+                self.force_close(guid, reason)
+
+        def force_close(self, guid: Union[str, list], reason: str = ''):
+            """强制关闭连接"""
+            if isinstance(guid, str):
+                guid = [guid]
+
+            for g in guid:
+                with self.lock:
+                    obj: OPCDA.OPCPyro = self.clients.pop(g, None)
+                    if obj is not None:
+                        obj.exit(reason)
+
+        def close_by_reason(self, reason: str = ''):
+            """根据原因事件分别关闭"""
+            try:
+                all_clients = self.get_clients()
+                if reason == 'limit':
+                    if len(all_clients) >= self.opc_config.OPC_DA_GATE_LIMIT_SIZE:
+                        reason = 'limit'
+                        stale_clients = sorted(all_clients, key=lambda s: s[2])[:-self.opc_config.OPC_DA_GATE_LIMIT_SIZE]
+                        self.force_close([client[0] for client in stale_clients], reason)
+                elif reason == 'timeout':
+                    stale_clients = [s for s in all_clients if (OPCDA.OPCCommon.get_timestamp() - s[2]) > self.opc_config.OPC_DA_GATE_TIMEOUT]
+                    self.force_close([client[0] for client in stale_clients], reason)
+                elif reason == 'exit':
+                    self.close_all_sessions(reason)
+            except Exception as e:
+                pass
+
+        def cleanup_clients(self, reasons: list):
+            for reason in reasons:
+                self.close_by_reason(reason)
+
+        def create_client(self):
+            """在Pyro服务器中创建新实例"""
+            if len(self.clients) > self.opc_config.OPC_DA_GATE_LIMIT_SIZE:
+                raise Exception(f"Connection reached maximum limit({self.opc_config.OPC_DA_GATE_LIMIT_SIZE})")
+
+            opc_da_client = OPCDA.OPCClient(self.opc_config.OPC_DA_CLASS, self.opc_config.OPC_DA_CLIENT_NAME)
+            uri = self._pyroDaemon.register(opc_da_client)
+            opc_client_id = uri.object
+            opc_da_client.set_svc_info(self.opc_config.OPC_DA_GATE_HOST, self.opc_config.OPC_DA_GATE_PORT, opc_client_id, self)
+            self.clients[opc_client_id] = OPCDA.OPCPyro(opc_client_id, Pyro5.client.current_context, opc_da_client)
+            return opc_da_client
+
+        def release_client(self, obj):
+            """在Pyro服务器中释放实例"""
+            if obj is not None:
+                self._pyroDaemon.unregister(obj)
+                with self.lock:
+                    self.clients.pop(obj.guid(), None)
+                del obj
+
+        def get_info(self) -> dict:
+            """获取进程信息"""
+            info: dict = dict()
+            info['config'] = self.opc_config.to_json()
+            info.update(OPCDA.OPCCommon.get_current_process())
+            return info
+
+        def restart(self):
+            """重启"""
+            return OPCDA.OPCCommon.restart_service(self.opc_config.OPC_DA_SERVICE_NAME)
+
+    class OPCPyroServer:
+
+        def __init__(self, opc_config):
+            self.opc_config = opc_config
+            self.pyro_daemon = None
+            self.pyro_event = Event()
+            self.pyro_thread = None
+            self.pyro_exit = False
+
+        def __del__(self):
+            self.exit()
+
+        def exit(self):
+            self.pyro_event.set()
+            if self.pyro_thread:
+                self.pyro_thread.join()
+            self.pyro_exit = True
+            if self.pyro_daemon:
+                self.pyro_daemon.shutdown()
+
+        def create_clean_thread(self):
+            self.pyro_thread = Thread(target=self.inactive_cleanup)
+            self.pyro_thread.start()
+
+        def delay(self, second: int):
+            while self.pyro_exit is False and second > 0:
+                self.pyro_event.wait(1)
+                second = second - 1
+
+        def inactive_cleanup(self):
+            """退出清除"""
+            pyro_server = None
+            while self.pyro_exit is False:
+                try:
+                    if pyro_server is None:
+                        pyro_server = OPCDA(self.opc_config.OPC_DA_GATE_HOST, self.opc_config.OPC_DA_GATE_PORT)
+                    self.delay(10)
+                    if self.pyro_event.is_set():
+                        pyro_server.cleanup_sessions(['exit'])
+                        self.pyro_event.clear()
+                        return
+                    else:
+                        pyro_server.cleanup_sessions(['timeout', 'limit'])
+                except Exception as e:
+                    logging.error(f"process({OPCDA.OPCCommon.get_current_pids()}): inactive_cleanup fail({e.__str__()})")
+                    pyro_server = None
+                    self.delay(30)
+
+        def run_loop(self):
+            self.pyro_daemon = Daemon(host=self.opc_config.OPC_DA_GATE_HOST, port=self.opc_config.OPC_DA_GATE_PORT)
+            self.pyro_daemon.register(OPCDA.OPCServer(self.opc_config), objectId="opc")
+            self.create_clean_thread()
+            self.pyro_daemon.requestLoop()
+
+        def run_foreground(self):
+            self.pyro_daemon = Daemon(host=self.opc_config.OPC_DA_GATE_HOST, port=self.opc_config.OPC_DA_GATE_PORT)
+            server = OPCDA.OPCServer(self.opc_config)
+            self.pyro_daemon.register(server, objectId="opc")
+            self.pyro_daemon.clientDisconnect = server.client_disconnected
+            self.create_clean_thread()
+            self.pyro_daemon.requestLoop()
 
     def __init__(self, host: Optional[str] = None, port: Optional[int] = None):
         self.host = 'localhost' if host is None else host
         self.port = 8810 if host is None else port
+        self.proxy = None
+
+    def __del__(self):
+        self.exit()
+
+    def exit(self):
+        if self.proxy is not None:
+            del self.proxy
+        self.proxy = None
+
+    def get_uri(self, prefix: str = 'PYRO:opc'):
+        return f"{prefix}@{self.host}:{self.port}"
+
+    def get_proxy(self, proxy_id: str = ''):
+        if self.proxy is None:
+            with Proxy(self.get_uri()) as proxy:
+                if len(proxy_id) > 0:
+                    proxy._pyroHandshake = proxy_id
+                    proxy._pyroBind()
+                self.proxy = proxy
+        return self.proxy
+
+    def call_method(self, func_name, *args, **kwargs):
+        proxy = self.get_proxy()
+        if hasattr(proxy, func_name):
+            return getattr(proxy, func_name)(*args, **kwargs)
+        raise Exception(f"call method({func_name}) fail")
 
     def get_sessions(self):
-        return Proxy(f"PYRO:opc@{self.host}:{self.port}").get_clients()
+        return self.get_proxy().get_clients()
 
     def close_session(self, guid):
-        return Proxy(f"PYRO:opc@{self.host}:{self.port}").force_close(guid)
+        return self.get_proxy().force_close(guid)
 
     def close_all_sessions(self):
-        return Proxy(f"PYRO:opc@{self.host}:{self.port}").close_all_sessions()
+        return self.get_proxy().close_all_sessions()
+
+    def cleanup_sessions(self, reasons: list):
+        return self.get_proxy().cleanup_clients(reasons)
 
     def open_client(self):
-        return Proxy(f"PYRO:opc@{self.host}:{self.port}").create_client()
+        client = self.get_proxy().create_client()
+        client.track_resource()
+        return client
 
     def get_info(self):
-        return Proxy(f"PYRO:opc@{self.host}:{self.port}").get_info()
+        return self.get_proxy().get_info()
 
     def restart(self):
-        return Proxy(f"PYRO:opc@{self.host}:{self.port}").restart()
+        return self.get_proxy().restart()
 
 
 class IOTOPCDA(IOTDriver):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.reinit()
 
     def reinit(self):
         self.exit_flag = False
-        IOTBaseCommon.function_thread(self.pump_wait_msg, False, f"opcda pump").start()
+        self.client = None
 
     def exit(self):
         self.exit_flag = True
         self.close()
         self.reinit()
 
     @classmethod
@@ -1132,39 +1628,39 @@
                 tag = point.get('point_tag')
                 result = self.get_device_property(self.configs.get('server'), tag, [self.get_write_quality, self.get_write_result])
             else:
                 result = [False, 'Point UnExist']
 
             results[name] = result
             if result[0] is not True:
-                self.logging(content=f"write value({name}) fail({result[1]})", level='ERROR', source=name, pos=self.stack_pos)
+                self.logging(content=f"write value({name}) fail({result[1]})", level='ERROR', source=name)
         return results
 
     def ping(self, **kwargs) -> bool:
         self.update_info(used=IOTBaseCommon.get_datetime_str())
-        return self._get_client() and self._get_client().ping()
+        return self._get_client() and self.client.ping()
 
     def scan(self, **kwargs):
         self.update_info(used=IOTBaseCommon.get_datetime_str())
         results = {}
         if self._get_client():
             path = kwargs.get('path', '*')
             include_property = kwargs.get('include_property', False)
-            self.logging(content=f"scan opc({path})", pos=self.stack_pos)
+            self.logging(content=f"scan opc({path})")
             points = self._get_client().list_items(paths=path, flat=True)  # flat=True
-            self.logging(content=f"scan opc flags({len(points)})", pos=self.stack_pos)
+            self.logging(content=f"scan opc flags({len(points)})")
             for point in points:
                 params = {'point_name': point, 'point_name_alias': point, 'point_writable': True, 'point_tag': point, 'point_type': '', 'point_description': '', 'point_value': ''}
                 if include_property is True:
                     properties = self._get_client().properties(tags=[point])
-                    self.logging(content=f"scan opc item({point}) property({len(properties)})", pos=self.stack_pos)
+                    self.logging(content=f"scan opc item({point}) property({len(properties)})")
                     for property in properties:
                         if len(property) >= 3:
                             if property[2] == 'Item Canonical DataType':
-                                params['point_type'] = str(property[3])
+                                params['point_type'] = OPCDA.VtType(property[3]).name
                             elif property[2] == 'Item Value':
                                 params['point_value'] = str(property[3])
                             elif property[2] == 'Item Description':
                                 params['point_description'] = property[3]
                 results[point] = self.create_point(**params)
         self.update_info(scan=len(results))
         return results
@@ -1185,64 +1681,59 @@
             host_info = host.split(':')
             if len(host_info) == 1:
                 return {'com': True, 'ip': host_info[0], 'port': None, 'server': self.configs.get('server'), 'group': self.configs.get('group')}
             elif len(host_info) == 2:
                 return {'com': False, 'ip': host_info[0], 'port': int(float(host_info[1])), 'server': self.configs.get('server'), 'group': self.configs.get('group')}
         return None
 
-    def _release_client(self, client):
+    def _release_client(self):
         try:
-            if client:
-                client.close()
+            if self.client:
+                self.client.close()
         except Exception as e:
             logging.error(f'release client fail({e.__str__()})')
         finally:
-            client = None
-        return None
+            self.client = None
 
     def _get_client(self, auto_connect: bool = True):
+        try:
+            if self.client:
+                if self.client.ping() is True:
+                    return self.client
+                self._release_client()
+        except Exception as e:
+            self.client = None
+
         if self.client is None:
             info = self._get_host_info()
             if isinstance(info, dict):
-                client = None
                 try:
                     if info.get('com') is True:
-                        client = OPCDA.OPCClient()
+                        self.client = OPCDA.OPCClient()
                     else:
-                        client = OPCDA(info.get('ip'), info.get('port')).open_client()
+                        self.client = OPCDA(info.get('ip'), info.get('port')).open_client()
 
                     if auto_connect is True:
-                        client.connect(info.get('server'), info.get('host'))
-                        self.logging(content=f"connect opc({info.get('host')}-{info.get('server')})", pos=self.stack_pos)
+                        self.client.connect(info.get('server'), info.get('host'))
+                        self.logging(content=f"connect opc({info.get('host')}-{info.get('server')})")
 
-                        client.add_group(self.configs.get('group'), self.configs.get('update_rate'))
-                        self.logging(content=f"add opc group({self.configs.get('group')})", pos=self.stack_pos)
+                        self.client.add_group(self.configs.get('group'), self.configs.get('update_rate'))
+                        self.logging(content=f"add opc group({self.configs.get('group')})")
                 except Exception as e:
-                    client = self._release_client(client)
+                    self._release_client()
                     raise e
-                self.client = client
         return self.client
 
-    def pump_wait_msg(self):
-        while self.exit_flag is False:
-            try:
-                if self.client is not None and self.client.is_connected() is True:
-                    pythoncom.PumpWaitingMessages()
-                    continue
-            except:
-                pass
-            time.sleep(0.1)
-
     def _read(self, tags: list):
         try:
             if len(tags) > 0 and self._get_client():
                 chunk_tags = IOTBaseCommon.chunk_list(tags, self.configs.get('read_limit', 100))
                 for chunk_tag in chunk_tags:
                     self.delay(0.0001)
-                    values = self._get_client().read(self.configs.get('group'), chunk_tag, self.configs.get('action'))
+                    values = self.client.read(self.configs.get('group'), chunk_tag, self.configs.get('action'))
                     for tag, value in values.items():
                         if isinstance(value, list):
                             if len(value) >= 4:
                                 (v, status, time, error, update) = value
                                 if status == 'Good':
                                     self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(True, v))
                                 else:
@@ -1266,21 +1757,20 @@
         except Exception as e:
             self.update_results(name, False, e.__str__())
         return None
 
     def _write(self, set_values: dict):
         try:
             if len(set_values) > 0 and self._get_client():
-                values = self._get_client().write(self.configs.get('group'), set_values)
+                values = self.client.write(self.configs.get('group'), set_values)
                 for tag, [status, result] in values.items():
                     self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(status, result, False))
         except Exception as e:
             for tag in set_values.keys():
                 self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(False, e.__str__(), False))
 
     def close(self):
-        if self.client is not None:
-            self.client = self._release_client(self.client)
+        self._release_client()
 
     def info(self, **kwargs):
         if self._get_client():
-            return self._get_client().get_info()
+            return self.client.get_info()
```

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.44/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/setup.py` & `RobertCommonDriver-0.1.44/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.43'
-DATE = '2023-06-12'
+VERSION = '0.1.44'
+DATE = '2023-07-14'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,70 @@
-import time
 import random
-from robertcommondriver.system.iot.iot_opcda import IOTOPCDA
+import time
+from robertcommondriver.system.iot.iot_plc_mitsubishi import MitsubishiClient, MitsubishiVersion, IOTPlcMitsubishi
 
 
 def logging_print(**kwargs):
     print(kwargs)
 
 
 def test_read_write():
-    dict_config = {
-        'server': 'Matrikon.OPC.Simulation.1',
-        'host': 'localhost',  # 'host': '192.168.1.36:8804', 192.168.2.131:8810
-        'enabled': True,
-        'group': f'opcda1',  #
-        'action': 'sync',
-        'read_limit': 50,
-        'update_rate': 500
-    }
+    omron = MitsubishiClient(MitsubishiVersion.Qna_3E, '192.168.1.12', 6000)
+    omron.logging(call_logging=logging_print)
+    while True:
+        aa = omron.read(('D263', 18))
+        print(aa)
+        #aa = omron.write(('D263', 18, 2.234))
+        #print(aa.contents[0].contents[8])
+        time.sleep(4)
 
-    dict_point = {}
-    dict_point['static_int'] = {'point_writable': True, 'point_name': 'static_int', 'point_tag': '213Bucket Brigade.Int1', 'point_type': '', 'point_description': ''}
-    dict_point['static_int1'] = {'point_writable': True, 'point_name': 'static_int1', 'point_tag': 'Bucket Brigade.Int1', 'point_type': '', 'point_description': ''}
-    dict_point['random_float'] = {'point_writable': True, 'point_name': 'random_float', 'point_tag': 'Random.Real4', 'point_type': '', 'point_description': ''}
-    dict_point['random_str'] = {'point_writable': True, 'point_name': 'random_str', 'point_tag': 'Random.String', 'point_type': '', 'point_description': ''}
 
-    client = IOTOPCDA(configs=dict_config, points=dict_point)
-    client.logging(call_logging=logging_print)
+def test_read_write1():
+    omron = MitsubishiClient(MitsubishiVersion.A_1E, '192.168.1.12', 6001)
+    omron.logging(call_logging=logging_print)
     while True:
-        try:
-            print(client.ping())
-            reuslts = client.read()
-            print(reuslts)
+        value = random.randint(1, 100) / 10
+        #value = 5.6
+        print(f"value: {value}")
+        a1 = omron.write(('D263', 18, value))
+        aa = omron.read(('D263', 18))
+        print(aa.contents[0].contents[8])
+        #aa = omron.write(('D263', 18, 2.234))
+        #print(aa.contents[0].contents[8])
+        time.sleep(4)
 
-            client.write(values={'static_int1': random.randint(1,10), 'static_int': random.randint(1,10)})
 
-            print(client.info())
-        except Exception as e:
-            client.close()
-            print(e.__str__())
+def test_read_write2():
+    omron = MitsubishiClient(MitsubishiVersion.Qna_3E, '192.168.1.12', 6000)
+    omron.logging(call_logging=logging_print)
+    while True:
+        value = random.randint(1, 100) / 10
+        #value = 5.6
+        print(f"value: {value}")
+        a1 = omron.write(('D263', 18, value))
+        aa = omron.read(('D263', 18))
+        print(aa.contents[0].contents[8])
+        #aa = omron.write(('D263', 18, 2.234))
+        #print(aa.contents[0].contents[8])
         time.sleep(4)
 
 
-def test_scan():
-    dict_config = {
-        'server': 'Matrikon.OPC.Simulation.1',
-        'host': 'localhost',  # 'host': '192.168.1.36:8804', 192.168.2.131:8810
-        'enabled': True,
-        'group': f'opcda1',  #
-        'read_limit': 50,
-        'update_rate': 500
-    }
-
+def test_iot_mistubishi_read():
+    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
     dict_point = {}
-
-    client = IOTOPCDA(configs=dict_config, points=dict_point)
+    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '2/192.168.1.12/6000', 'point_address': 'D263', 'point_type': 18, 'point_scale': '1'}
+    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '2/192.168.1.12/6000', 'point_address': 'D260', 'point_type': 18, 'point_scale': '1'}
+    client = IOTPlcMitsubishi(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
-    # print(f"ping: {client.ping()}")
-    print(f"discover: {client.discover()}")
-    result = client.scan(path='*', include_property=True)
-    print(f"scan: {result}")
-    time.sleep(4)
+    while True:
+        try:
+            aa = client.write(values={'plc10': random.randint(1, 100) / 10})
+            print(aa)
+
+            re = client.read()
+            print(re)
+        except Exception as e:
+            print(f"error: {e.__str__()}")
+        time.sleep(4)
 
 
-test_read_write()
+test_iot_mistubishi_read()
```

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.44/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

