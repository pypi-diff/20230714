# Comparing `tmp/spyc_iot-0.0.1.tar.gz` & `tmp/spyc_iot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyc_iot-0.0.1.tar", last modified: Fri Jul 14 06:06:19 2023, max compression
+gzip compressed data, was "spyc_iot-0.0.2.tar", last modified: Fri Jul 14 06:16:31 2023, max compression
```

## Comparing `spyc_iot-0.0.1.tar` & `spyc_iot-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:06:19.434629 spyc_iot-0.0.1/
--rw-rw-rw-   0        0        0     1072 2023-07-14 04:21:51.000000 spyc_iot-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      358 2023-07-14 06:06:19.435627 spyc_iot-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-14 04:24:10.000000 spyc_iot-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      474 2023-07-14 06:06:19.436625 spyc_iot-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 06:06:19.415081 spyc_iot-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 06:06:19.421066 spyc_iot-0.0.1/src/spyc_iot/
--rw-rw-rw-   0        0        0       58 2023-07-14 05:58:38.000000 spyc_iot-0.0.1/src/spyc_iot/__init__.py
--rw-rw-rw-   0        0        0      667 2023-07-14 05:55:28.000000 spyc_iot-0.0.1/src/spyc_iot/ntp.py
--rw-rw-rw-   0        0        0      505 2023-07-14 04:50:45.000000 spyc_iot-0.0.1/src/spyc_iot/wifi.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:06:19.434629 spyc_iot-0.0.1/src/spyc_iot.egg-info/
--rw-rw-rw-   0        0        0      358 2023-07-14 06:06:19.000000 spyc_iot-0.0.1/src/spyc_iot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-14 06:06:19.000000 spyc_iot-0.0.1/src/spyc_iot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:06:19.000000 spyc_iot-0.0.1/src/spyc_iot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 06:06:19.000000 spyc_iot-0.0.1/src/spyc_iot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 06:16:31.295180 spyc_iot-0.0.2/
+-rw-rw-rw-   0        0        0     1072 2023-07-14 04:21:51.000000 spyc_iot-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      307 2023-07-14 06:16:31.295180 spyc_iot-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-14 04:24:10.000000 spyc_iot-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      417 2023-07-14 06:16:31.300166 spyc_iot-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 06:16:31.276231 spyc_iot-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 06:16:31.281218 spyc_iot-0.0.2/src/spyc_iot/
+-rw-rw-rw-   0        0        0       58 2023-07-14 05:58:38.000000 spyc_iot-0.0.2/src/spyc_iot/__init__.py
+-rw-rw-rw-   0        0        0      667 2023-07-14 05:55:28.000000 spyc_iot-0.0.2/src/spyc_iot/ntp.py
+-rw-rw-rw-   0        0        0      505 2023-07-14 04:50:45.000000 spyc_iot-0.0.2/src/spyc_iot/wifi.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:16:31.294182 spyc_iot-0.0.2/src/spyc_iot.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-07-14 06:16:31.000000 spyc_iot-0.0.2/src/spyc_iot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-14 06:16:31.000000 spyc_iot-0.0.2/src/spyc_iot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:16:31.000000 spyc_iot-0.0.2/src/spyc_iot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 06:16:31.000000 spyc_iot-0.0.2/src/spyc_iot.egg-info/top_level.txt
```

### Comparing `spyc_iot-0.0.1/LICENSE` & `spyc_iot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spyc_iot-0.0.1/src/spyc_iot/ntp.py` & `spyc_iot-0.0.2/src/spyc_iot/ntp.py`

 * *Files identical despite different names*

