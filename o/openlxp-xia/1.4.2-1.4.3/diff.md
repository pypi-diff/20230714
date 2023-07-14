# Comparing `tmp/openlxp-xia-1.4.2.tar.gz` & `tmp/openlxp-xia-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlxp-xia-1.4.2.tar", last modified: Wed May 17 20:56:22 2023, max compression
+gzip compressed data, was "openlxp-xia-1.4.3.tar", last modified: Fri Jul 14 18:30:11 2023, max compression
```

## Comparing `openlxp-xia-1.4.2.tar` & `openlxp-xia-1.4.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.408792 openlxp-xia-1.4.2/
--rw-r--r--   0 jametobin   (502) staff       (20)     4930 2023-05-17 20:56:22.408936 openlxp-xia-1.4.2/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)     4064 2023-05-16 21:32:06.000000 openlxp-xia-1.4.2/README.md
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.335478 openlxp-xia-1.4.2/openlxp_xia/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)     1945 2023-05-17 19:45:41.000000 openlxp-xia-1.4.2/openlxp_xia/admin.py
--rw-r--r--   0 jametobin   (502) staff       (20)      147 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/apps.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.347993 openlxp-xia-1.4.2/openlxp_xia/management/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/__init__.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.359310 openlxp-xia-1.4.2/openlxp_xia/management/commands/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/commands/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)     4718 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/commands/load_supplemental_metadata.py
--rw-r--r--   0 jametobin   (502) staff       (20)     4403 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/commands/load_target_metadata.py
--rw-r--r--   0 jametobin   (502) staff       (20)    12029 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/commands/transform_source_metadata.py
--rw-r--r--   0 jametobin   (502) staff       (20)     5116 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/commands/validate_source_metadata.py
--rw-r--r--   0 jametobin   (502) staff       (20)     7956 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/commands/validate_target_metadata.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.369135 openlxp-xia-1.4.2/openlxp_xia/management/utils/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/utils/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)     9840 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/management/utils/xia_internal.py
--rw-r--r--   0 jametobin   (502) staff       (20)     2087 2023-05-17 20:55:25.000000 openlxp-xia-1.4.2/openlxp_xia/management/utils/xis_client.py
--rw-r--r--   0 jametobin   (502) staff       (20)     5117 2023-05-16 20:05:42.000000 openlxp-xia-1.4.2/openlxp_xia/management/utils/xss_client.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.383180 openlxp-xia-1.4.2/openlxp_xia/migrations/
--rw-r--r--   0 jametobin   (502) staff       (20)     7683 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/migrations/0001_initial.py
--rw-r--r--   0 jametobin   (502) staff       (20)     1726 2023-05-16 20:05:42.000000 openlxp-xia-1.4.2/openlxp_xia/migrations/0002_use_xss.py
--rw-r--r--   0 jametobin   (502) staff       (20)      487 2023-05-17 13:46:33.000000 openlxp-xia-1.4.2/openlxp_xia/migrations/0003_xisconfiguration_xis_api_key.py
--rw-r--r--   0 jametobin   (502) staff       (20)      444 2023-05-17 20:55:59.000000 openlxp-xia-1.4.2/openlxp_xia/migrations/0004_alter_xiaconfiguration_xss_api.py
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/migrations/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)    10669 2023-05-17 18:48:19.000000 openlxp-xia-1.4.2/openlxp_xia/models.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.400048 openlxp-xia-1.4.2/openlxp_xia/tests/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/tests/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)    17232 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/tests/test_setup.py
--rw-r--r--   0 jametobin   (502) staff       (20)    27386 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_command_intergration.py
--rw-r--r--   0 jametobin   (502) staff       (20)    33612 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_command_unit.py
--rw-r--r--   0 jametobin   (502) staff       (20)     1120 2023-05-16 20:05:42.000000 openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_models_integration.py
--rw-r--r--   0 jametobin   (502) staff       (20)    12993 2023-05-16 20:05:42.000000 openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_models_unit.py
--rw-r--r--   0 jametobin   (502) staff       (20)      710 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_utils_integration.py
--rw-r--r--   0 jametobin   (502) staff       (20)    22425 2023-05-16 20:05:42.000000 openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_utils_unit.py
--rw-r--r--   0 jametobin   (502) staff       (20)      761 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/urls.py
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia/views.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.347109 openlxp-xia-1.4.2/openlxp_xia.egg-info/
--rw-r--r--   0 jametobin   (502) staff       (20)     4930 2023-05-17 20:56:22.000000 openlxp-xia-1.4.2/openlxp_xia.egg-info/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)     1599 2023-05-17 20:56:22.000000 openlxp-xia-1.4.2/openlxp_xia.egg-info/SOURCES.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        1 2023-05-17 20:56:22.000000 openlxp-xia-1.4.2/openlxp_xia.egg-info/dependency_links.txt
--rw-r--r--   0 jametobin   (502) staff       (20)       14 2023-05-17 20:56:22.000000 openlxp-xia-1.4.2/openlxp_xia.egg-info/requires.txt
--rw-r--r--   0 jametobin   (502) staff       (20)       45 2023-05-17 20:56:22.000000 openlxp-xia-1.4.2/openlxp_xia.egg-info/top_level.txt
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-17 20:56:22.408236 openlxp-xia-1.4.2/openlxp_xia_project/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia_project/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)      415 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia_project/asgi.py
--rw-r--r--   0 jametobin   (502) staff       (20)     4540 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia_project/settings.py
--rw-r--r--   0 jametobin   (502) staff       (20)      761 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia_project/urls.py
--rw-r--r--   0 jametobin   (502) staff       (20)      415 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/openlxp_xia_project/wsgi.py
--rw-r--r--   0 jametobin   (502) staff       (20)      974 2023-05-17 20:56:22.409455 openlxp-xia-1.4.2/setup.cfg
--rw-r--r--   0 jametobin   (502) staff       (20)       95 2022-06-24 18:54:06.000000 openlxp-xia-1.4.2/setup.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.824203 openlxp-xia-1.4.3/
+-rw-r--r--   0 jametobin   (502) staff       (20)     4930 2023-07-14 18:30:11.824351 openlxp-xia-1.4.3/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     4064 2023-05-16 21:32:06.000000 openlxp-xia-1.4.3/README.md
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.788765 openlxp-xia-1.4.3/openlxp_xia/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     1945 2023-05-17 19:45:41.000000 openlxp-xia-1.4.3/openlxp_xia/admin.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      147 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/apps.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.796561 openlxp-xia-1.4.3/openlxp_xia/management/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/__init__.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.802784 openlxp-xia-1.4.3/openlxp_xia/management/commands/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/commands/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     4718 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/commands/load_supplemental_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     4403 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/commands/load_target_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    12029 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/commands/transform_source_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     5116 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/commands/validate_source_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     7956 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/commands/validate_target_metadata.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.805213 openlxp-xia-1.4.3/openlxp_xia/management/utils/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/utils/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     9840 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/management/utils/xia_internal.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     2087 2023-05-17 20:55:25.000000 openlxp-xia-1.4.3/openlxp_xia/management/utils/xis_client.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     5117 2023-05-16 20:05:42.000000 openlxp-xia-1.4.3/openlxp_xia/management/utils/xss_client.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.811669 openlxp-xia-1.4.3/openlxp_xia/migrations/
+-rw-r--r--   0 jametobin   (502) staff       (20)     7683 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/migrations/0001_initial.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     1726 2023-05-16 20:05:42.000000 openlxp-xia-1.4.3/openlxp_xia/migrations/0002_use_xss.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      487 2023-05-17 13:46:33.000000 openlxp-xia-1.4.3/openlxp_xia/migrations/0003_xisconfiguration_xis_api_key.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      444 2023-05-17 20:55:59.000000 openlxp-xia-1.4.3/openlxp_xia/migrations/0004_alter_xiaconfiguration_xss_api.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      454 2023-07-14 16:10:59.000000 openlxp-xia-1.4.3/openlxp_xia/migrations/0005_alter_xisconfiguration_xis_api_key.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/migrations/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    10670 2023-07-14 16:11:06.000000 openlxp-xia-1.4.3/openlxp_xia/models.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.819049 openlxp-xia-1.4.3/openlxp_xia/tests/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/tests/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    17232 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/tests/test_setup.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    27386 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_command_intergration.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    33612 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_command_unit.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     1120 2023-05-16 20:05:42.000000 openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_models_integration.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    12993 2023-05-16 20:05:42.000000 openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_models_unit.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      710 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_utils_integration.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    22425 2023-05-16 20:05:42.000000 openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_utils_unit.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      761 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/urls.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia/views.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.795889 openlxp-xia-1.4.3/openlxp_xia.egg-info/
+-rw-r--r--   0 jametobin   (502) staff       (20)     4930 2023-07-14 18:30:11.000000 openlxp-xia-1.4.3/openlxp_xia.egg-info/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     1665 2023-07-14 18:30:11.000000 openlxp-xia-1.4.3/openlxp_xia.egg-info/SOURCES.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        1 2023-07-14 18:30:11.000000 openlxp-xia-1.4.3/openlxp_xia.egg-info/dependency_links.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       14 2023-07-14 18:30:11.000000 openlxp-xia-1.4.3/openlxp_xia.egg-info/requires.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       45 2023-07-14 18:30:11.000000 openlxp-xia-1.4.3/openlxp_xia.egg-info/top_level.txt
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-07-14 18:30:11.823675 openlxp-xia-1.4.3/openlxp_xia_project/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia_project/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      415 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia_project/asgi.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     4540 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia_project/settings.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      761 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia_project/urls.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      415 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/openlxp_xia_project/wsgi.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      974 2023-07-14 18:30:11.825281 openlxp-xia-1.4.3/setup.cfg
+-rw-r--r--   0 jametobin   (502) staff       (20)       95 2022-06-24 18:54:06.000000 openlxp-xia-1.4.3/setup.py
```

### Comparing `openlxp-xia-1.4.2/PKG-INFO` & `openlxp-xia-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-xia
-Version: 1.4.2
+Version: 1.4.3
 Summary: Sample installable XIA
 Home-page: https://github.com/OpenLXP/openlxp-xia/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `openlxp-xia-1.4.2/README.md` & `openlxp-xia-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/admin.py` & `openlxp-xia-1.4.3/openlxp_xia/admin.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/commands/load_supplemental_metadata.py` & `openlxp-xia-1.4.3/openlxp_xia/management/commands/load_supplemental_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/commands/load_target_metadata.py` & `openlxp-xia-1.4.3/openlxp_xia/management/commands/load_target_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/commands/transform_source_metadata.py` & `openlxp-xia-1.4.3/openlxp_xia/management/commands/transform_source_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/commands/validate_source_metadata.py` & `openlxp-xia-1.4.3/openlxp_xia/management/commands/validate_source_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/commands/validate_target_metadata.py` & `openlxp-xia-1.4.3/openlxp_xia/management/commands/validate_target_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/utils/xia_internal.py` & `openlxp-xia-1.4.3/openlxp_xia/management/utils/xia_internal.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/utils/xis_client.py` & `openlxp-xia-1.4.3/openlxp_xia/management/utils/xis_client.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/management/utils/xss_client.py` & `openlxp-xia-1.4.3/openlxp_xia/management/utils/xss_client.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/migrations/0001_initial.py` & `openlxp-xia-1.4.3/openlxp_xia/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/migrations/0002_use_xss.py` & `openlxp-xia-1.4.3/openlxp_xia/migrations/0002_use_xss.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/models.py` & `openlxp-xia-1.4.3/openlxp_xia/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     xis_supplemental_api_endpoint = models.CharField(
         help_text='Enter the XIS Supplemental Ledger API endpoint',
         max_length=200
     )
 
     xis_api_key = models.CharField(
         help_text="Enter the XIS API Key",
-        max_length=40
+        max_length=128
     )
 
     def save(self, *args, **kwargs):
         if not self.pk and XISConfiguration.objects.exists():
             raise ValidationError('There can be only one XISConfiguration '
                                   'instance')
         return super(XISConfiguration, self).save(*args, **kwargs)
```

### Comparing `openlxp-xia-1.4.2/openlxp_xia/tests/test_setup.py` & `openlxp-xia-1.4.3/openlxp_xia/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_command_intergration.py` & `openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_command_intergration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_command_unit.py` & `openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_command_unit.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_models_integration.py` & `openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_models_integration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_models_unit.py` & `openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_models_unit.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_utils_integration.py` & `openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_utils_integration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/tests/test_xia_utils_unit.py` & `openlxp-xia-1.4.3/openlxp_xia/tests/test_xia_utils_unit.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia/urls.py` & `openlxp-xia-1.4.3/openlxp_xia/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia.egg-info/PKG-INFO` & `openlxp-xia-1.4.3/openlxp_xia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-xia
-Version: 1.4.2
+Version: 1.4.3
 Summary: Sample installable XIA
 Home-page: https://github.com/OpenLXP/openlxp-xia/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `openlxp-xia-1.4.2/openlxp_xia.egg-info/SOURCES.txt` & `openlxp-xia-1.4.3/openlxp_xia.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 openlxp_xia/management/utils/xia_internal.py
 openlxp_xia/management/utils/xis_client.py
 openlxp_xia/management/utils/xss_client.py
 openlxp_xia/migrations/0001_initial.py
 openlxp_xia/migrations/0002_use_xss.py
 openlxp_xia/migrations/0003_xisconfiguration_xis_api_key.py
 openlxp_xia/migrations/0004_alter_xiaconfiguration_xss_api.py
+openlxp_xia/migrations/0005_alter_xisconfiguration_xis_api_key.py
 openlxp_xia/migrations/__init__.py
 openlxp_xia/tests/__init__.py
 openlxp_xia/tests/test_setup.py
 openlxp_xia/tests/test_xia_command_intergration.py
 openlxp_xia/tests/test_xia_command_unit.py
 openlxp_xia/tests/test_xia_models_integration.py
 openlxp_xia/tests/test_xia_models_unit.py
```

### Comparing `openlxp-xia-1.4.2/openlxp_xia_project/settings.py` & `openlxp-xia-1.4.3/openlxp_xia_project/settings.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/openlxp_xia_project/urls.py` & `openlxp-xia-1.4.3/openlxp_xia_project/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.2/setup.cfg` & `openlxp-xia-1.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openlxp-xia
-version = 1.4.2
+version = 1.4.3
 description = Sample installable XIA
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/OpenLXP/openlxp-xia/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
```

