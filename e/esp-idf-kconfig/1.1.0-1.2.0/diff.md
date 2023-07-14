# Comparing `tmp/esp-idf-kconfig-1.1.0.tar.gz` & `tmp/esp-idf-kconfig-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-kconfig/esp-idf-kconfig/dist/.tmp-28w21jig/esp-idf-kconfig-1.1.0.tar", last modified: Mon Dec 12 18:25:06 2022, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-kconfig/esp-idf-kconfig/dist/.tmp-bqzexah1/esp-idf-kconfig-1.2.0.tar", last modified: Fri Jul 14 17:20:17 2023, max compression
```

## Comparing `esp-idf-kconfig-1.1.0.tar` & `esp-idf-kconfig-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18164 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig/gen_kconfig_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/esp_idf_kconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/kconfgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/kconfgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/kconfgen/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25976 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/kconfgen/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/kconfserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/kconfserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/kconfserver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/kconfserver/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 18:25:06.000000 esp-idf-kconfig-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2022-12-12 18:24:50.000000 esp-idf-kconfig-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18164 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig/gen_kconfig_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/esp_idf_kconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/kconfgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/kconfgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/kconfgen/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26146 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/kconfgen/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/kconfserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/kconfserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/kconfserver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/kconfserver/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:20:17.000000 esp-idf-kconfig-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-14 17:19:52.000000 esp-idf-kconfig-1.2.0/setup.py
```

### Comparing `esp-idf-kconfig-1.1.0/LICENSE` & `esp-idf-kconfig-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-kconfig-1.1.0/PKG-INFO` & `esp-idf-kconfig-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-kconfig
-Version: 1.1.0
+Version: 1.2.0
 Summary: Kconfig tooling for esp-idf
 Home-page: https://github.com/espressif/esp-idf-kconfig
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,configuration,kconfig
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-kconfig-1.1.0/esp_idf_kconfig/gen_kconfig_doc.py` & `esp-idf-kconfig-1.2.0/esp_idf_kconfig/gen_kconfig_doc.py`

 * *Files identical despite different names*

### Comparing `esp-idf-kconfig-1.1.0/esp_idf_kconfig.egg-info/PKG-INFO` & `esp-idf-kconfig-1.2.0/esp_idf_kconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-kconfig
-Version: 1.1.0
+Version: 1.2.0
 Summary: Kconfig tooling for esp-idf
 Home-page: https://github.com/espressif/esp-idf-kconfig
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,configuration,kconfig
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-kconfig-1.1.0/kconfgen/core.py` & `esp-idf-kconfig-1.2.0/kconfgen/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Command line tool to take in ESP-IDF sdkconfig files with project
 # settings and output data in multiple formats (update config, generate
 # header file, generate .cmake include file, documentation, etc).
 #
 # Used internally by the ESP-IDF build system. But designed to be
 # non-IDF-specific.
 #
-# SPDX-FileCopyrightText: 2018-2021 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2018-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import json
 import os
 import os.path
 import re
@@ -405,38 +405,38 @@
             try:
                 os.remove(temp_file)
             except OSError:
                 pass
 
 
 def write_config(deprecated_options, config, filename):
-    CONFIG_HEADING = """#
+    idf_version = os.environ.get("IDF_VERSION", "")
+    CONFIG_HEADING = f"""#
 # Automatically generated file. DO NOT EDIT.
-# Espressif IoT Development Framework (ESP-IDF) Project Configuration
+# Espressif IoT Development Framework (ESP-IDF) {idf_version} Project Configuration
 #
 """
     config.write_config(filename, header=CONFIG_HEADING)
     deprecated_options.append_config(config, filename)
 
 
 def write_min_config(deprecated_options, config, filename):
+    idf_version = os.environ.get("IDF_VERSION", "")
     target_symbol = config.syms["IDF_TARGET"]
     # 'esp32` is harcoded here because the default value of IDF_TARGET is set on the first run from the environment
     # variable. I.E. `esp32  is not defined as default value.
     write_target = target_symbol.str_value != "esp32"
 
     CONFIG_HEADING = textwrap.dedent(
-        """\
+        f"""\
     # This file was generated using idf.py save-defconfig. It can be edited manually.
-    # Espressif IoT Development Framework (ESP-IDF) Project Minimal Configuration
+    # Espressif IoT Development Framework (ESP-IDF) {idf_version} Project Minimal Configuration
     #
-    {}\
-    """.format(
-            target_symbol.config_string if write_target else ""
-        )
+    {target_symbol.config_string if write_target else ""}\
+    """
     )
 
     # convert `# CONFIG_XY is not set` to `CONFIG_XY=n` to improve readability
     lines = config._min_config_contents(header=CONFIG_HEADING).splitlines()
     unset_match = re.compile(
         r"# {}([^ ]+) is not set".format(config.config_prefix)
     ).match
@@ -445,17 +445,18 @@
         if match:
             lines[idx] = f"{config.config_prefix}{match.group(1)}=n"
     lines[-1] += "\n"
     config._write_if_changed(filename, "\n".join(lines))
 
 
 def write_header(deprecated_options, config, filename):
-    CONFIG_HEADING = """/*
+    idf_version = os.environ.get("IDF_VERSION", "")
+    CONFIG_HEADING = f"""/*
  * Automatically generated file. DO NOT EDIT.
- * Espressif IoT Development Framework (ESP-IDF) Configuration Header
+ * Espressif IoT Development Framework (ESP-IDF) {idf_version} Configuration Header
  */
 #pragma once
 """
     config.write_autoconf(filename, header=CONFIG_HEADING)
     deprecated_options.append_header(config, filename)
```

### Comparing `esp-idf-kconfig-1.1.0/kconfserver/core.py` & `esp-idf-kconfig-1.2.0/kconfserver/core.py`

 * *Files identical despite different names*

### Comparing `esp-idf-kconfig-1.1.0/setup.py` & `esp-idf-kconfig-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,17 +40,14 @@
     long_description=get_long_description(),
     url="https://github.com/espressif/esp-idf-kconfig",
     packages=find_packages(),
     python_requires=">=3.7",
     install_requires=_install_requires,
     extras_require={
         "dev": [
-            "flake8>=3.2.0",
-            "flake8-import-order",
-            "black",
             "pre-commit",
             "pexpect",
         ],
     },
     keywords=["espressif", "embedded", "project", "configuration", "kconfig"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

