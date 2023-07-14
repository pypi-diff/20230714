# Comparing `tmp/unitelabs_sila-0.1.1.tar.gz` & `tmp/unitelabs_sila-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitelabs_sila-0.1.1.tar", max compression
+gzip compressed data, was "unitelabs_sila-0.1.2.tar", max compression
```

## Comparing `unitelabs_sila-0.1.1.tar` & `unitelabs_sila-0.1.2.tar`

### file list

```diff
@@ -1,117 +1,118 @@
--rw-r--r--   0        0        0     1069 2023-06-08 22:13:58.281937 unitelabs_sila-0.1.1/LICENSE
--rw-r--r--   0        0        0     2038 2023-06-14 08:42:29.964140 unitelabs_sila-0.1.1/README.md
--rw-r--r--   0        0        0     1945 2023-06-18 10:00:10.921604 unitelabs_sila-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      106 2023-06-14 07:16:21.186838 unitelabs_sila-0.1.1/src/sila/__init__.py
--rw-r--r--   0        0        0      146 2023-06-08 22:13:58.442811 unitelabs_sila-0.1.1/src/sila/cloud_connector/__init__.py
--rw-r--r--   0        0        0    17225 2023-06-16 16:19:03.239630 unitelabs_sila-0.1.1/src/sila/cloud_connector/cloud_server_endpoint.py
--rw-r--r--   0        0        0    10246 2023-06-10 15:36:21.353326 unitelabs_sila-0.1.1/src/sila/cloud_connector/messages.py
--rw-r--r--   0        0        0      592 2023-06-10 15:37:02.130746 unitelabs_sila-0.1.1/src/sila/commands/__init__.py
--rw-r--r--   0        0        0      946 2023-06-16 13:18:07.658640 unitelabs_sila-0.1.1/src/sila/commands/command.py
--rw-r--r--   0        0        0     1147 2023-06-11 21:57:12.512348 unitelabs_sila-0.1.1/src/sila/commands/command_confirmation.py
--rw-r--r--   0        0        0     4709 2023-06-16 16:19:20.467543 unitelabs_sila-0.1.1/src/sila/commands/command_execution.py
--rw-r--r--   0        0        0     3046 2023-06-11 21:57:12.517685 unitelabs_sila-0.1.1/src/sila/commands/command_execution_info.py
--rw-r--r--   0        0        0      453 2023-06-11 21:57:12.518337 unitelabs_sila-0.1.1/src/sila/commands/command_execution_uuid.py
--rw-r--r--   0        0        0      616 2023-06-11 21:57:12.521234 unitelabs_sila-0.1.1/src/sila/commands/observable_command.py
--rw-r--r--   0        0        0      390 2023-06-11 21:57:12.522401 unitelabs_sila-0.1.1/src/sila/commands/unobservable_command.py
--rw-r--r--   0        0        0     1231 2023-06-13 17:34:19.443118 unitelabs_sila-0.1.1/src/sila/constraints/__init__.py
--rw-r--r--   0        0        0      625 2023-06-11 21:57:12.523714 unitelabs_sila-0.1.1/src/sila/constraints/allowed_types.py
--rw-r--r--   0        0        0      478 2023-06-14 05:05:30.931848 unitelabs_sila-0.1.1/src/sila/constraints/constraint.py
--rw-r--r--   0        0        0      921 2023-06-08 08:41:46.740250 unitelabs_sila-0.1.1/src/sila/constraints/content_type.py
--rw-r--r--   0        0        0      889 2023-06-03 09:51:05.606924 unitelabs_sila-0.1.1/src/sila/constraints/element_count.py
--rw-r--r--   0        0        0     1555 2023-06-16 13:19:36.970594 unitelabs_sila-0.1.1/src/sila/constraints/fully_qualified_identifier.py
--rw-r--r--   0        0        0      934 2023-06-11 21:57:12.525011 unitelabs_sila-0.1.1/src/sila/constraints/length.py
--rw-r--r--   0        0        0      904 2023-06-03 09:51:05.610073 unitelabs_sila-0.1.1/src/sila/constraints/maximal_element_count.py
--rw-r--r--   0        0        0      888 2023-06-03 09:55:31.158596 unitelabs_sila-0.1.1/src/sila/constraints/maximal_exclusive.py
--rw-r--r--   0        0        0      907 2023-06-03 09:55:36.776856 unitelabs_sila-0.1.1/src/sila/constraints/maximal_inclusive.py
--rw-r--r--   0        0        0      985 2023-06-14 05:03:54.580670 unitelabs_sila-0.1.1/src/sila/constraints/maximal_length.py
--rw-r--r--   0        0        0      899 2023-06-03 09:51:05.614671 unitelabs_sila-0.1.1/src/sila/constraints/minimal_element_count.py
--rw-r--r--   0        0        0      893 2023-06-03 09:55:34.058872 unitelabs_sila-0.1.1/src/sila/constraints/minimal_exclusive.py
--rw-r--r--   0        0        0      909 2023-06-03 09:55:38.301758 unitelabs_sila-0.1.1/src/sila/constraints/minimal_inclusive.py
--rw-r--r--   0        0        0      994 2023-06-03 09:51:05.622353 unitelabs_sila-0.1.1/src/sila/constraints/minimal_length.py
--rw-r--r--   0        0        0      623 2023-06-14 05:05:30.933163 unitelabs_sila-0.1.1/src/sila/constraints/pattern.py
--rw-r--r--   0        0        0      665 2023-06-08 08:53:44.725620 unitelabs_sila-0.1.1/src/sila/constraints/schema.py
--rw-r--r--   0        0        0      726 2023-06-03 09:55:39.422718 unitelabs_sila-0.1.1/src/sila/constraints/set.py
--rw-r--r--   0        0        0     1602 2023-06-08 08:29:13.185856 unitelabs_sila-0.1.1/src/sila/constraints/unit.py
--rw-r--r--   0        0        0      144 2023-06-11 21:57:12.526082 unitelabs_sila-0.1.1/src/sila/core/__init__.py
--rw-r--r--   0        0        0     3851 2023-06-16 16:35:01.561541 unitelabs_sila-0.1.1/src/sila/core/feature.py
--rw-r--r--   0        0        0     1709 2023-06-11 21:57:12.527474 unitelabs_sila-0.1.1/src/sila/core/handler.py
--rw-r--r--   0        0        0     2971 2023-06-14 05:05:30.933915 unitelabs_sila-0.1.1/src/sila/core/server.py
--rw-r--r--   0        0        0      769 2023-06-13 15:55:13.097999 unitelabs_sila-0.1.1/src/sila/data_types/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-04 19:54:04.417061 unitelabs_sila-0.1.1/src/sila/data_types/any.py
--rw-r--r--   0        0        0     1053 2023-06-07 19:30:07.082139 unitelabs_sila-0.1.1/src/sila/data_types/basic_type.py
--rw-r--r--   0        0        0     1354 2023-06-04 20:29:24.951615 unitelabs_sila-0.1.1/src/sila/data_types/binary.py
--rw-r--r--   0        0        0      771 2023-06-04 19:48:34.281597 unitelabs_sila-0.1.1/src/sila/data_types/boolean.py
--rw-r--r--   0        0        0     1336 2023-06-07 19:30:18.487002 unitelabs_sila-0.1.1/src/sila/data_types/constrained.py
--rw-r--r--   0        0        0      867 2023-06-07 19:30:26.689597 unitelabs_sila-0.1.1/src/sila/data_types/data_type.py
--rw-r--r--   0        0        0     2644 2023-06-16 10:08:28.352141 unitelabs_sila-0.1.1/src/sila/data_types/data_type_definition.py
--rw-r--r--   0        0        0     1965 2023-06-04 19:47:40.030909 unitelabs_sila-0.1.1/src/sila/data_types/date.py
--rw-r--r--   0        0        0     1130 2023-06-04 19:46:07.096305 unitelabs_sila-0.1.1/src/sila/data_types/duration.py
--rw-r--r--   0        0        0      743 2023-06-05 10:53:18.827154 unitelabs_sila-0.1.1/src/sila/data_types/integer.py
--rw-r--r--   0        0        0     1286 2023-06-07 19:30:34.932708 unitelabs_sila-0.1.1/src/sila/data_types/list.py
--rw-r--r--   0        0        0      760 2023-06-04 19:38:15.675710 unitelabs_sila-0.1.1/src/sila/data_types/real.py
--rw-r--r--   0        0        0     1147 2023-06-08 22:12:52.848122 unitelabs_sila-0.1.1/src/sila/data_types/string.py
--rw-r--r--   0        0        0     4271 2023-06-09 10:45:44.390563 unitelabs_sila-0.1.1/src/sila/data_types/structure.py
--rw-r--r--   0        0        0     1948 2023-06-04 19:45:25.161612 unitelabs_sila-0.1.1/src/sila/data_types/time.py
--rw-r--r--   0        0        0     2533 2023-06-04 19:44:26.791814 unitelabs_sila-0.1.1/src/sila/data_types/timestamp.py
--rw-r--r--   0        0        0     1250 2023-06-04 19:42:37.697579 unitelabs_sila-0.1.1/src/sila/data_types/timezone.py
--rw-r--r--   0        0        0      659 2023-06-04 19:42:08.651066 unitelabs_sila-0.1.1/src/sila/data_types/void.py
--rw-r--r--   0        0        0      164 2023-06-08 20:52:53.907366 unitelabs_sila-0.1.1/src/sila/datetime/__init__.py
--rw-r--r--   0        0        0     2262 2023-06-08 22:13:58.286982 unitelabs_sila-0.1.1/src/sila/datetime/date.py
--rw-r--r--   0        0        0       64 2023-06-08 22:13:58.443800 unitelabs_sila-0.1.1/src/sila/discovery/__init__.py
--rw-r--r--   0        0        0     1785 2023-06-08 22:13:58.444125 unitelabs_sila-0.1.1/src/sila/discovery/broadcaster.py
--rw-r--r--   0        0        0      446 2023-06-05 20:09:27.499133 unitelabs_sila-0.1.1/src/sila/errors/__init__.py
--rw-r--r--   0        0        0     2508 2023-06-16 10:02:45.842808 unitelabs_sila-0.1.1/src/sila/errors/defined_execution_error.py
--rw-r--r--   0        0        0     2005 2023-06-05 20:08:43.148208 unitelabs_sila-0.1.1/src/sila/errors/framework_error.py
--rw-r--r--   0        0        0     1808 2023-06-05 20:10:27.279204 unitelabs_sila-0.1.1/src/sila/errors/sila_error.py
--rw-r--r--   0        0        0      647 2023-06-05 20:10:05.335814 unitelabs_sila-0.1.1/src/sila/errors/sila_exception.py
--rw-r--r--   0        0        0      908 2023-06-05 20:10:02.365590 unitelabs_sila-0.1.1/src/sila/errors/undefined_execution_error.py
--rw-r--r--   0        0        0     1282 2023-06-05 20:09:59.865569 unitelabs_sila-0.1.1/src/sila/errors/validation_error.py
--rw-r--r--   0        0        0      941 2023-06-09 06:33:45.337996 unitelabs_sila-0.1.1/src/sila/fdl_parser/__init__.py
--rw-r--r--   0        0        0     1684 2023-06-08 11:09:33.254085 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_command.py
--rw-r--r--   0        0        0     5095 2023-06-08 22:13:58.338287 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_constraint.py
--rw-r--r--   0        0        0     3182 2023-06-08 10:47:41.040745 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type.py
--rw-r--r--   0        0        0      752 2023-06-09 06:36:56.248348 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type_definition.py
--rw-r--r--   0        0        0      586 2023-06-08 10:46:24.525760 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_defined_execution_error.py
--rw-r--r--   0        0        0      418 2023-06-08 09:45:35.011949 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_defined_execution_error_list.py
--rw-r--r--   0        0        0      245 2023-06-09 18:55:45.433970 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_description.py
--rw-r--r--   0        0        0     2496 2023-06-16 13:37:39.864064 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_feature.py
--rw-r--r--   0        0        0      852 2023-06-08 22:13:58.339752 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_metadata.py
--rw-r--r--   0        0        0      944 2023-06-08 11:09:39.444072 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_property.py
--rw-r--r--   0        0        0      760 2023-06-08 10:43:45.918520 unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_sila_element.py
--rw-r--r--   0        0        0     1211 2023-06-04 15:05:41.890867 unitelabs_sila-0.1.1/src/sila/identifiers/__init__.py
--rw-r--r--   0        0        0      921 2023-06-16 10:01:09.883882 unitelabs_sila-0.1.1/src/sila/identifiers/command_identifier.py
--rw-r--r--   0        0        0     1010 2023-06-16 10:01:09.885217 unitelabs_sila-0.1.1/src/sila/identifiers/command_parameter_identifier.py
--rw-r--r--   0        0        0      997 2023-06-16 10:01:09.885723 unitelabs_sila-0.1.1/src/sila/identifiers/command_response_identifier.py
--rw-r--r--   0        0        0     1037 2023-06-16 10:01:09.886355 unitelabs_sila-0.1.1/src/sila/identifiers/custom_data_type_identifier.py
--rw-r--r--   0        0        0     1139 2023-06-16 10:01:09.887826 unitelabs_sila-0.1.1/src/sila/identifiers/defined_execution_error_identifier.py
--rw-r--r--   0        0        0     1696 2023-06-16 13:21:37.926999 unitelabs_sila-0.1.1/src/sila/identifiers/feature_identifier.py
--rw-r--r--   0        0        0     1009 2023-06-16 10:39:35.807691 unitelabs_sila-0.1.1/src/sila/identifiers/identifier.py
--rw-r--r--   0        0        0     1177 2023-06-16 10:01:09.902704 unitelabs_sila-0.1.1/src/sila/identifiers/intermediate_command_response_identifier.py
--rw-r--r--   0        0        0      923 2023-06-16 10:39:06.952069 unitelabs_sila-0.1.1/src/sila/identifiers/metadata_identifier.py
--rw-r--r--   0        0        0      925 2023-06-16 10:01:09.904485 unitelabs_sila-0.1.1/src/sila/identifiers/property_identifier.py
--rw-r--r--   0        0        0       55 2023-06-08 22:13:58.340262 unitelabs_sila-0.1.1/src/sila/metadata/__init__.py
--rw-r--r--   0        0        0     2850 2023-06-16 10:01:44.723784 unitelabs_sila-0.1.1/src/sila/metadata/metadata.py
--rw-r--r--   0        0        0      224 2023-06-05 14:34:27.247039 unitelabs_sila-0.1.1/src/sila/properties/__init__.py
--rw-r--r--   0        0        0      395 2023-06-05 18:28:34.990277 unitelabs_sila-0.1.1/src/sila/properties/observable_property.py
--rw-r--r--   0        0        0     1313 2023-06-16 10:01:53.702668 unitelabs_sila-0.1.1/src/sila/properties/property.py
--rw-r--r--   0        0        0      389 2023-06-05 18:29:02.534670 unitelabs_sila-0.1.1/src/sila/properties/unobservable_property.py
--rw-r--r--   0        0        0      550 2023-06-05 05:48:33.521128 unitelabs_sila-0.1.1/src/sila/protobuf/__init__.py
--rw-r--r--   0        0        0      441 2023-06-03 09:48:32.882854 unitelabs_sila-0.1.1/src/sila/protobuf/decode_error.py
--rw-r--r--   0        0        0        0 2023-06-12 07:48:23.932059 unitelabs_sila-0.1.1/src/sila/py.typed
--rw-r--r--   0        0        0      670 2023-06-08 22:13:58.341251 unitelabs_sila-0.1.1/src/sila/server/__init__.py
--rw-r--r--   0        0        0     1913 2023-06-16 10:38:43.335380 unitelabs_sila-0.1.1/src/sila/server/feature.py
--rw-r--r--   0        0        0      862 2023-06-07 10:04:20.415702 unitelabs_sila-0.1.1/src/sila/server/handler.py
--rw-r--r--   0        0        0     1374 2023-06-15 20:32:32.072752 unitelabs_sila-0.1.1/src/sila/server/metadata.py
--rw-r--r--   0        0        0     8240 2023-06-16 08:24:39.138382 unitelabs_sila-0.1.1/src/sila/server/observable_command.py
--rw-r--r--   0        0        0     2925 2023-06-15 20:28:56.560208 unitelabs_sila-0.1.1/src/sila/server/observable_property.py
--rw-r--r--   0        0        0     5302 2023-06-16 16:25:47.002998 unitelabs_sila-0.1.1/src/sila/server/server.py
--rw-r--r--   0        0        0     2504 2023-06-16 13:26:00.125295 unitelabs_sila-0.1.1/src/sila/server/unobservable_command.py
--rw-r--r--   0        0        0     2638 2023-06-15 20:29:13.265509 unitelabs_sila-0.1.1/src/sila/server/unobservable_property.py
--rw-r--r--   0        0        0      222 2023-06-14 05:05:30.935366 unitelabs_sila-0.1.1/src/sila/validators/__init__.py
--rw-r--r--   0        0        0      963 2023-06-14 05:05:30.935791 unitelabs_sila-0.1.1/src/sila/validators/display_name.py
--rw-r--r--   0        0        0     1192 2023-06-14 05:05:30.936233 unitelabs_sila-0.1.1/src/sila/validators/domain.py
--rw-r--r--   0        0        0     1335 2023-06-14 05:05:30.936778 unitelabs_sila-0.1.1/src/sila/validators/identifier.py
--rw-r--r--   0        0        0     1129 2023-06-14 05:05:30.937160 unitelabs_sila-0.1.1/src/sila/validators/uuid.py
--rw-r--r--   0        0        0     1347 2023-06-14 05:05:30.937529 unitelabs_sila-0.1.1/src/sila/validators/validator.py
--rw-r--r--   0        0        0     2901 2023-06-14 05:05:30.937980 unitelabs_sila-0.1.1/src/sila/validators/version.py
--rw-r--r--   0        0        0     3469 1970-01-01 00:00:00.000000 unitelabs_sila-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-08 22:13:58.281937 unitelabs_sila-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2038 2023-06-14 08:42:29.964140 unitelabs_sila-0.1.2/README.md
+-rw-r--r--   0        0        0     1969 2023-07-14 12:49:50.425011 unitelabs_sila-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-06-14 07:16:21.186838 unitelabs_sila-0.1.2/src/sila/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-08 22:13:58.442811 unitelabs_sila-0.1.2/src/sila/cloud_connector/__init__.py
+-rw-r--r--   0        0        0    17261 2023-07-14 12:48:34.469413 unitelabs_sila-0.1.2/src/sila/cloud_connector/cloud_server_endpoint.py
+-rw-r--r--   0        0        0    10246 2023-06-10 15:36:21.353326 unitelabs_sila-0.1.2/src/sila/cloud_connector/messages.py
+-rw-r--r--   0        0        0      592 2023-06-10 15:37:02.130746 unitelabs_sila-0.1.2/src/sila/commands/__init__.py
+-rw-r--r--   0        0        0      946 2023-06-16 13:18:07.658640 unitelabs_sila-0.1.2/src/sila/commands/command.py
+-rw-r--r--   0        0        0     1147 2023-06-11 21:57:12.512348 unitelabs_sila-0.1.2/src/sila/commands/command_confirmation.py
+-rw-r--r--   0        0        0     4709 2023-06-18 10:20:22.602675 unitelabs_sila-0.1.2/src/sila/commands/command_execution.py
+-rw-r--r--   0        0        0     3046 2023-06-11 21:57:12.517685 unitelabs_sila-0.1.2/src/sila/commands/command_execution_info.py
+-rw-r--r--   0        0        0      453 2023-06-11 21:57:12.518337 unitelabs_sila-0.1.2/src/sila/commands/command_execution_uuid.py
+-rw-r--r--   0        0        0      616 2023-06-11 21:57:12.521234 unitelabs_sila-0.1.2/src/sila/commands/observable_command.py
+-rw-r--r--   0        0        0      390 2023-06-11 21:57:12.522401 unitelabs_sila-0.1.2/src/sila/commands/unobservable_command.py
+-rw-r--r--   0        0        0     1231 2023-06-13 17:34:19.443118 unitelabs_sila-0.1.2/src/sila/constraints/__init__.py
+-rw-r--r--   0        0        0      625 2023-06-11 21:57:12.523714 unitelabs_sila-0.1.2/src/sila/constraints/allowed_types.py
+-rw-r--r--   0        0        0      478 2023-06-14 05:05:30.931848 unitelabs_sila-0.1.2/src/sila/constraints/constraint.py
+-rw-r--r--   0        0        0      921 2023-06-08 08:41:46.740250 unitelabs_sila-0.1.2/src/sila/constraints/content_type.py
+-rw-r--r--   0        0        0      889 2023-06-03 09:51:05.606924 unitelabs_sila-0.1.2/src/sila/constraints/element_count.py
+-rw-r--r--   0        0        0     1555 2023-06-16 13:19:36.970594 unitelabs_sila-0.1.2/src/sila/constraints/fully_qualified_identifier.py
+-rw-r--r--   0        0        0      934 2023-06-11 21:57:12.525011 unitelabs_sila-0.1.2/src/sila/constraints/length.py
+-rw-r--r--   0        0        0      904 2023-06-03 09:51:05.610073 unitelabs_sila-0.1.2/src/sila/constraints/maximal_element_count.py
+-rw-r--r--   0        0        0      888 2023-06-03 09:55:31.158596 unitelabs_sila-0.1.2/src/sila/constraints/maximal_exclusive.py
+-rw-r--r--   0        0        0      907 2023-06-03 09:55:36.776856 unitelabs_sila-0.1.2/src/sila/constraints/maximal_inclusive.py
+-rw-r--r--   0        0        0      985 2023-06-14 05:03:54.580670 unitelabs_sila-0.1.2/src/sila/constraints/maximal_length.py
+-rw-r--r--   0        0        0      899 2023-06-03 09:51:05.614671 unitelabs_sila-0.1.2/src/sila/constraints/minimal_element_count.py
+-rw-r--r--   0        0        0      893 2023-06-03 09:55:34.058872 unitelabs_sila-0.1.2/src/sila/constraints/minimal_exclusive.py
+-rw-r--r--   0        0        0      909 2023-06-03 09:55:38.301758 unitelabs_sila-0.1.2/src/sila/constraints/minimal_inclusive.py
+-rw-r--r--   0        0        0      994 2023-06-03 09:51:05.622353 unitelabs_sila-0.1.2/src/sila/constraints/minimal_length.py
+-rw-r--r--   0        0        0      623 2023-06-14 05:05:30.933163 unitelabs_sila-0.1.2/src/sila/constraints/pattern.py
+-rw-r--r--   0        0        0      665 2023-06-08 08:53:44.725620 unitelabs_sila-0.1.2/src/sila/constraints/schema.py
+-rw-r--r--   0        0        0      726 2023-06-03 09:55:39.422718 unitelabs_sila-0.1.2/src/sila/constraints/set.py
+-rw-r--r--   0        0        0     1602 2023-06-08 08:29:13.185856 unitelabs_sila-0.1.2/src/sila/constraints/unit.py
+-rw-r--r--   0        0        0      144 2023-06-11 21:57:12.526082 unitelabs_sila-0.1.2/src/sila/core/__init__.py
+-rw-r--r--   0        0        0     3851 2023-06-18 10:20:22.603573 unitelabs_sila-0.1.2/src/sila/core/feature.py
+-rw-r--r--   0        0        0     1709 2023-06-11 21:57:12.527474 unitelabs_sila-0.1.2/src/sila/core/handler.py
+-rw-r--r--   0        0        0     2971 2023-06-14 05:05:30.933915 unitelabs_sila-0.1.2/src/sila/core/server.py
+-rw-r--r--   0        0        0      769 2023-06-13 15:55:13.097999 unitelabs_sila-0.1.2/src/sila/data_types/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-04 19:54:04.417061 unitelabs_sila-0.1.2/src/sila/data_types/any.py
+-rw-r--r--   0        0        0     1053 2023-06-07 19:30:07.082139 unitelabs_sila-0.1.2/src/sila/data_types/basic_type.py
+-rw-r--r--   0        0        0     1354 2023-06-04 20:29:24.951615 unitelabs_sila-0.1.2/src/sila/data_types/binary.py
+-rw-r--r--   0        0        0      771 2023-06-04 19:48:34.281597 unitelabs_sila-0.1.2/src/sila/data_types/boolean.py
+-rw-r--r--   0        0        0     1336 2023-06-07 19:30:18.487002 unitelabs_sila-0.1.2/src/sila/data_types/constrained.py
+-rw-r--r--   0        0        0      867 2023-06-07 19:30:26.689597 unitelabs_sila-0.1.2/src/sila/data_types/data_type.py
+-rw-r--r--   0        0        0     2561 2023-06-19 12:26:05.062889 unitelabs_sila-0.1.2/src/sila/data_types/data_type_definition.py
+-rw-r--r--   0        0        0     1965 2023-06-04 19:47:40.030909 unitelabs_sila-0.1.2/src/sila/data_types/date.py
+-rw-r--r--   0        0        0     1130 2023-06-04 19:46:07.096305 unitelabs_sila-0.1.2/src/sila/data_types/duration.py
+-rw-r--r--   0        0        0      743 2023-06-05 10:53:18.827154 unitelabs_sila-0.1.2/src/sila/data_types/integer.py
+-rw-r--r--   0        0        0     1286 2023-06-07 19:30:34.932708 unitelabs_sila-0.1.2/src/sila/data_types/list.py
+-rw-r--r--   0        0        0      760 2023-06-04 19:38:15.675710 unitelabs_sila-0.1.2/src/sila/data_types/real.py
+-rw-r--r--   0        0        0     1147 2023-06-08 22:12:52.848122 unitelabs_sila-0.1.2/src/sila/data_types/string.py
+-rw-r--r--   0        0        0     4239 2023-06-19 12:26:05.063650 unitelabs_sila-0.1.2/src/sila/data_types/structure.py
+-rw-r--r--   0        0        0     1948 2023-06-04 19:45:25.161612 unitelabs_sila-0.1.2/src/sila/data_types/time.py
+-rw-r--r--   0        0        0     2533 2023-06-04 19:44:26.791814 unitelabs_sila-0.1.2/src/sila/data_types/timestamp.py
+-rw-r--r--   0        0        0     1250 2023-06-04 19:42:37.697579 unitelabs_sila-0.1.2/src/sila/data_types/timezone.py
+-rw-r--r--   0        0        0      659 2023-06-04 19:42:08.651066 unitelabs_sila-0.1.2/src/sila/data_types/void.py
+-rw-r--r--   0        0        0      164 2023-06-08 20:52:53.907366 unitelabs_sila-0.1.2/src/sila/datetime/__init__.py
+-rw-r--r--   0        0        0     2262 2023-06-08 22:13:58.286982 unitelabs_sila-0.1.2/src/sila/datetime/date.py
+-rw-r--r--   0        0        0      100 2023-07-14 12:48:34.470445 unitelabs_sila-0.1.2/src/sila/discovery/__init__.py
+-rw-r--r--   0        0        0     3160 2023-07-14 12:48:34.471207 unitelabs_sila-0.1.2/src/sila/discovery/broadcaster.py
+-rw-r--r--   0        0        0      446 2023-06-05 20:09:27.499133 unitelabs_sila-0.1.2/src/sila/errors/__init__.py
+-rw-r--r--   0        0        0     2508 2023-06-16 10:02:45.842808 unitelabs_sila-0.1.2/src/sila/errors/defined_execution_error.py
+-rw-r--r--   0        0        0     2005 2023-06-05 20:08:43.148208 unitelabs_sila-0.1.2/src/sila/errors/framework_error.py
+-rw-r--r--   0        0        0     1808 2023-06-05 20:10:27.279204 unitelabs_sila-0.1.2/src/sila/errors/sila_error.py
+-rw-r--r--   0        0        0      647 2023-06-05 20:10:05.335814 unitelabs_sila-0.1.2/src/sila/errors/sila_exception.py
+-rw-r--r--   0        0        0      908 2023-06-05 20:10:02.365590 unitelabs_sila-0.1.2/src/sila/errors/undefined_execution_error.py
+-rw-r--r--   0        0        0     1282 2023-06-05 20:09:59.865569 unitelabs_sila-0.1.2/src/sila/errors/validation_error.py
+-rw-r--r--   0        0        0      941 2023-06-09 06:33:45.337996 unitelabs_sila-0.1.2/src/sila/fdl_parser/__init__.py
+-rw-r--r--   0        0        0     1684 2023-06-08 11:09:33.254085 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_command.py
+-rw-r--r--   0        0        0     5095 2023-06-08 22:13:58.338287 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_constraint.py
+-rw-r--r--   0        0        0     3182 2023-06-08 10:47:41.040745 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_data_type.py
+-rw-r--r--   0        0        0      752 2023-06-09 06:36:56.248348 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_data_type_definition.py
+-rw-r--r--   0        0        0      586 2023-06-08 10:46:24.525760 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_defined_execution_error.py
+-rw-r--r--   0        0        0      418 2023-06-08 09:45:35.011949 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_defined_execution_error_list.py
+-rw-r--r--   0        0        0      245 2023-06-09 18:55:45.433970 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_description.py
+-rw-r--r--   0        0        0     2496 2023-06-18 10:20:22.605181 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_feature.py
+-rw-r--r--   0        0        0      852 2023-06-08 22:13:58.339752 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_metadata.py
+-rw-r--r--   0        0        0      944 2023-06-08 11:09:39.444072 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_property.py
+-rw-r--r--   0        0        0      760 2023-06-08 10:43:45.918520 unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_sila_element.py
+-rw-r--r--   0        0        0     1211 2023-06-04 15:05:41.890867 unitelabs_sila-0.1.2/src/sila/identifiers/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-16 10:01:09.883882 unitelabs_sila-0.1.2/src/sila/identifiers/command_identifier.py
+-rw-r--r--   0        0        0     1010 2023-06-16 10:01:09.885217 unitelabs_sila-0.1.2/src/sila/identifiers/command_parameter_identifier.py
+-rw-r--r--   0        0        0      997 2023-06-16 10:01:09.885723 unitelabs_sila-0.1.2/src/sila/identifiers/command_response_identifier.py
+-rw-r--r--   0        0        0     1037 2023-06-16 10:01:09.886355 unitelabs_sila-0.1.2/src/sila/identifiers/custom_data_type_identifier.py
+-rw-r--r--   0        0        0     1139 2023-06-16 10:01:09.887826 unitelabs_sila-0.1.2/src/sila/identifiers/defined_execution_error_identifier.py
+-rw-r--r--   0        0        0     1696 2023-06-18 10:20:22.606148 unitelabs_sila-0.1.2/src/sila/identifiers/feature_identifier.py
+-rw-r--r--   0        0        0     1009 2023-06-18 10:20:22.607496 unitelabs_sila-0.1.2/src/sila/identifiers/identifier.py
+-rw-r--r--   0        0        0     1177 2023-06-16 10:01:09.902704 unitelabs_sila-0.1.2/src/sila/identifiers/intermediate_command_response_identifier.py
+-rw-r--r--   0        0        0      923 2023-06-16 10:39:06.952069 unitelabs_sila-0.1.2/src/sila/identifiers/metadata_identifier.py
+-rw-r--r--   0        0        0      925 2023-06-16 10:01:09.904485 unitelabs_sila-0.1.2/src/sila/identifiers/property_identifier.py
+-rw-r--r--   0        0        0       55 2023-06-08 22:13:58.340262 unitelabs_sila-0.1.2/src/sila/metadata/__init__.py
+-rw-r--r--   0        0        0     2850 2023-06-16 10:01:44.723784 unitelabs_sila-0.1.2/src/sila/metadata/metadata.py
+-rw-r--r--   0        0        0      224 2023-06-05 14:34:27.247039 unitelabs_sila-0.1.2/src/sila/properties/__init__.py
+-rw-r--r--   0        0        0      395 2023-06-05 18:28:34.990277 unitelabs_sila-0.1.2/src/sila/properties/observable_property.py
+-rw-r--r--   0        0        0     1313 2023-06-16 10:01:53.702668 unitelabs_sila-0.1.2/src/sila/properties/property.py
+-rw-r--r--   0        0        0      389 2023-06-05 18:29:02.534670 unitelabs_sila-0.1.2/src/sila/properties/unobservable_property.py
+-rw-r--r--   0        0        0      550 2023-06-05 05:48:33.521128 unitelabs_sila-0.1.2/src/sila/protobuf/__init__.py
+-rw-r--r--   0        0        0      441 2023-06-03 09:48:32.882854 unitelabs_sila-0.1.2/src/sila/protobuf/decode_error.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:48:23.932059 unitelabs_sila-0.1.2/src/sila/py.typed
+-rw-r--r--   0        0        0      743 2023-07-14 12:48:34.471947 unitelabs_sila-0.1.2/src/sila/server/__init__.py
+-rw-r--r--   0        0        0     2441 2023-07-14 12:48:34.472439 unitelabs_sila-0.1.2/src/sila/server/encryption.py
+-rw-r--r--   0        0        0     1913 2023-06-18 10:20:22.608544 unitelabs_sila-0.1.2/src/sila/server/feature.py
+-rw-r--r--   0        0        0      862 2023-06-07 10:04:20.415702 unitelabs_sila-0.1.2/src/sila/server/handler.py
+-rw-r--r--   0        0        0     1374 2023-06-18 10:20:22.609468 unitelabs_sila-0.1.2/src/sila/server/metadata.py
+-rw-r--r--   0        0        0     8240 2023-06-19 11:56:43.549022 unitelabs_sila-0.1.2/src/sila/server/observable_command.py
+-rw-r--r--   0        0        0     2925 2023-06-18 10:20:22.610974 unitelabs_sila-0.1.2/src/sila/server/observable_property.py
+-rw-r--r--   0        0        0     6232 2023-07-14 12:48:34.473195 unitelabs_sila-0.1.2/src/sila/server/server.py
+-rw-r--r--   0        0        0     2504 2023-06-18 10:20:22.612390 unitelabs_sila-0.1.2/src/sila/server/unobservable_command.py
+-rw-r--r--   0        0        0     2638 2023-06-18 10:20:22.613258 unitelabs_sila-0.1.2/src/sila/server/unobservable_property.py
+-rw-r--r--   0        0        0      222 2023-06-14 05:05:30.935366 unitelabs_sila-0.1.2/src/sila/validators/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-14 05:05:30.935791 unitelabs_sila-0.1.2/src/sila/validators/display_name.py
+-rw-r--r--   0        0        0     1192 2023-06-14 05:05:30.936233 unitelabs_sila-0.1.2/src/sila/validators/domain.py
+-rw-r--r--   0        0        0     1335 2023-06-14 05:05:30.936778 unitelabs_sila-0.1.2/src/sila/validators/identifier.py
+-rw-r--r--   0        0        0     1129 2023-06-14 05:05:30.937160 unitelabs_sila-0.1.2/src/sila/validators/uuid.py
+-rw-r--r--   0        0        0     1347 2023-06-14 05:05:30.937529 unitelabs_sila-0.1.2/src/sila/validators/validator.py
+-rw-r--r--   0        0        0     2901 2023-06-14 05:05:30.937980 unitelabs_sila-0.1.2/src/sila/validators/version.py
+-rw-r--r--   0        0        0     3469 1970-01-01 00:00:00.000000 unitelabs_sila-0.1.2/PKG-INFO
```

### Comparing `unitelabs_sila-0.1.1/LICENSE` & `unitelabs_sila-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/README.md` & `unitelabs_sila-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/pyproject.toml` & `unitelabs_sila-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitelabs-sila"
-version = "0.1.1"
+version = "0.1.2"
 description = "An un-opinionated SiLA 2 library."
 license = "MIT"
 authors = ["UniteLabs AG <developers+sila@unitelabs.ch>"]
 readme = "README.md"
 homepage = "https://sila-standard.com"
 repository = "https://gitlab.com/unitelabs/integrations/sila2/sila-python"
 documentation = "https://gitlab.com/unitelabs/integrations/sila2/sila-python/-/tree/main/docs/"
@@ -33,14 +33,15 @@
 python = "^3.9"
 grpcio = "1.54.2"
 pure-protobuf = "3.0.0a5"
 zeroconf = "0.64.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
+cryptography = "41.0.2"
 isort = "5.12.0"
 pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.1.0"
 
 [tool.black]
```

### Comparing `unitelabs_sila-0.1.1/src/sila/cloud_connector/cloud_server_endpoint.py` & `unitelabs_sila-0.1.2/src/sila/cloud_connector/cloud_server_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 import logging
 import typing
 import weakref
 
 import grpc
 import grpc.aio
 import grpc.experimental
+import typing_extensions
 
 from sila import commands, errors
 from sila.server import ObservableCommand, ObservableProperty, Server, UnobservableCommand, UnobservableProperty
 
 from . import messages
 
 
-class CloudServerEndpointConfig(typing.TypedDict, total=False):
+class CloudServerEndpointConfig(typing_extensions.TypedDict, total=False):
     endpoint: str
     secure: bool
 
 
 class Context:
     _callback: typing.Optional[typing.Callable] = None
     running = False
```

### Comparing `unitelabs_sila-0.1.1/src/sila/cloud_connector/messages.py` & `unitelabs_sila-0.1.2/src/sila/cloud_connector/messages.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/commands/__init__.py` & `unitelabs_sila-0.1.2/src/sila/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/commands/command.py` & `unitelabs_sila-0.1.2/src/sila/commands/command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/commands/command_confirmation.py` & `unitelabs_sila-0.1.2/src/sila/commands/command_confirmation.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/commands/command_execution.py` & `unitelabs_sila-0.1.2/src/sila/commands/command_execution.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/commands/command_execution_info.py` & `unitelabs_sila-0.1.2/src/sila/commands/command_execution_info.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/commands/observable_command.py` & `unitelabs_sila-0.1.2/src/sila/commands/observable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/__init__.py` & `unitelabs_sila-0.1.2/src/sila/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/allowed_types.py` & `unitelabs_sila-0.1.2/src/sila/constraints/allowed_types.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/content_type.py` & `unitelabs_sila-0.1.2/src/sila/constraints/content_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/element_count.py` & `unitelabs_sila-0.1.2/src/sila/constraints/element_count.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/fully_qualified_identifier.py` & `unitelabs_sila-0.1.2/src/sila/constraints/fully_qualified_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/length.py` & `unitelabs_sila-0.1.2/src/sila/constraints/length.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/maximal_element_count.py` & `unitelabs_sila-0.1.2/src/sila/constraints/maximal_element_count.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/maximal_exclusive.py` & `unitelabs_sila-0.1.2/src/sila/constraints/maximal_exclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/maximal_inclusive.py` & `unitelabs_sila-0.1.2/src/sila/constraints/maximal_inclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/maximal_length.py` & `unitelabs_sila-0.1.2/src/sila/constraints/maximal_length.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/minimal_element_count.py` & `unitelabs_sila-0.1.2/src/sila/constraints/minimal_element_count.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/minimal_exclusive.py` & `unitelabs_sila-0.1.2/src/sila/constraints/minimal_exclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/minimal_inclusive.py` & `unitelabs_sila-0.1.2/src/sila/constraints/minimal_inclusive.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/minimal_length.py` & `unitelabs_sila-0.1.2/src/sila/constraints/minimal_length.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/pattern.py` & `unitelabs_sila-0.1.2/src/sila/constraints/pattern.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/schema.py` & `unitelabs_sila-0.1.2/src/sila/constraints/schema.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/set.py` & `unitelabs_sila-0.1.2/src/sila/constraints/set.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/constraints/unit.py` & `unitelabs_sila-0.1.2/src/sila/constraints/unit.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/core/feature.py` & `unitelabs_sila-0.1.2/src/sila/core/feature.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/core/handler.py` & `unitelabs_sila-0.1.2/src/sila/core/handler.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/core/server.py` & `unitelabs_sila-0.1.2/src/sila/core/server.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/__init__.py` & `unitelabs_sila-0.1.2/src/sila/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/any.py` & `unitelabs_sila-0.1.2/src/sila/data_types/any.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/basic_type.py` & `unitelabs_sila-0.1.2/src/sila/data_types/basic_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/binary.py` & `unitelabs_sila-0.1.2/src/sila/data_types/binary.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/boolean.py` & `unitelabs_sila-0.1.2/src/sila/data_types/boolean.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/constrained.py` & `unitelabs_sila-0.1.2/src/sila/data_types/constrained.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/data_type.py` & `unitelabs_sila-0.1.2/src/sila/data_types/data_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/data_type_definition.py` & `unitelabs_sila-0.1.2/src/sila/data_types/data_type_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,14 @@
     """Human readable name of the custom data type."""
 
     description: str = dataclasses.field(repr=False, default="")
     """Describes the use and purpose of the custom data type."""
 
     data_type: dataclasses.InitVar[DataType] = Void()
 
-    factory: typing.Callable = dataclasses.field(repr=False, default=lambda: ...)
-
     feature: core.Feature | None = dataclasses.field(repr=False, default=None)
 
     def __post_init__(self, data_type: DataType):
         self.message = Structure(
             elements=[
                 Structure.Element(
                     identifier=self.identifier,
```

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/date.py` & `unitelabs_sila-0.1.2/src/sila/data_types/date.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/duration.py` & `unitelabs_sila-0.1.2/src/sila/data_types/duration.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/integer.py` & `unitelabs_sila-0.1.2/src/sila/data_types/integer.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/list.py` & `unitelabs_sila-0.1.2/src/sila/data_types/list.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/real.py` & `unitelabs_sila-0.1.2/src/sila/data_types/real.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/string.py` & `unitelabs_sila-0.1.2/src/sila/data_types/string.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/structure.py` & `unitelabs_sila-0.1.2/src/sila/data_types/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,23 +38,24 @@
 
     Element: typing.ClassVar = Element
 
     elements: list[Structure.Element] = dataclasses.field(default_factory=list)
 
     def __post_init__(self):
         self.__elements_by_identifier = {
-            element.identifier.lower(): (index + 1, element) for index, element in enumerate(self.elements)
+            element.identifier: (index + 1, element) for index, element in enumerate(self.elements)
         }
 
     def encode(self, value: dict, field_number: int | None = None) -> bytes:
         stream = io.BytesIO()
         chunks = bytearray()
 
         for key, item in value.items():
-            index, field = self.__elements_by_identifier[key.lower().replace("_", "")]
+            index, field = self.__elements_by_identifier[key]
+
             if field is None:
                 continue
 
             data = field.data_type.encode(item, field_number=index)
             if not isinstance(field.data_type, List):
                 chunks.append(protobuf.Tag(field_number=index, wire_type=protobuf.WireType.LEN).encode())
                 t = io.BytesIO()
```

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/time.py` & `unitelabs_sila-0.1.2/src/sila/data_types/time.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/timestamp.py` & `unitelabs_sila-0.1.2/src/sila/data_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/timezone.py` & `unitelabs_sila-0.1.2/src/sila/data_types/timezone.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/data_types/void.py` & `unitelabs_sila-0.1.2/src/sila/data_types/void.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/datetime/date.py` & `unitelabs_sila-0.1.2/src/sila/datetime/date.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/errors/defined_execution_error.py` & `unitelabs_sila-0.1.2/src/sila/errors/defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/errors/framework_error.py` & `unitelabs_sila-0.1.2/src/sila/errors/framework_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/errors/sila_error.py` & `unitelabs_sila-0.1.2/src/sila/errors/sila_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/errors/sila_exception.py` & `unitelabs_sila-0.1.2/src/sila/errors/sila_exception.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/errors/undefined_execution_error.py` & `unitelabs_sila-0.1.2/src/sila/errors/undefined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/errors/validation_error.py` & `unitelabs_sila-0.1.2/src/sila/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/__init__.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_command.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_constraint.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_constraint.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_data_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_data_type_definition.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_data_type_definition.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_defined_execution_error.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_feature.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_feature.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_metadata.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_metadata.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_property.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/fdl_parser/serialize_sila_element.py` & `unitelabs_sila-0.1.2/src/sila/fdl_parser/serialize_sila_element.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/__init__.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/command_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/command_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/command_parameter_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/command_parameter_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/command_response_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/command_response_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/custom_data_type_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/custom_data_type_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/defined_execution_error_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/defined_execution_error_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/feature_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/feature_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/intermediate_command_response_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/intermediate_command_response_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/metadata_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/metadata_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/identifiers/property_identifier.py` & `unitelabs_sila-0.1.2/src/sila/identifiers/property_identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/metadata/metadata.py` & `unitelabs_sila-0.1.2/src/sila/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/properties/property.py` & `unitelabs_sila-0.1.2/src/sila/properties/property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/protobuf/__init__.py` & `unitelabs_sila-0.1.2/src/sila/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/server/feature.py` & `unitelabs_sila-0.1.2/src/sila/server/feature.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/server/handler.py` & `unitelabs_sila-0.1.2/src/sila/server/handler.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/server/metadata.py` & `unitelabs_sila-0.1.2/src/sila/server/metadata.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/server/observable_command.py` & `unitelabs_sila-0.1.2/src/sila/server/observable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/server/observable_property.py` & `unitelabs_sila-0.1.2/src/sila/server/observable_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/server/server.py` & `unitelabs_sila-0.1.2/src/sila/server/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,41 @@
 
 import asyncio
 import logging
 import typing
 import uuid
 
 import grpc.aio
+import typing_extensions
 
 from sila import commands, core, identifiers
 
 if typing.TYPE_CHECKING:
     from .feature import Feature
 
 
-class ServerConfig(typing.TypedDict, total=False):
+class ServerConfig(typing_extensions.TypedDict, total=False):
     host: str
     """Bind the gRPC server to this host."""
 
     port: typing.Union[str, int]
     """Bind the gRPC server to this port. If set to `0` an available port is chosen at runtime."""
 
+    tls: bool
+    """
+    Whether to enable TLS based encryption. If enabled, a `cert` and `key` pair need to be provided.
+    Defaults to `False`.
+    """
+
+    cert: bytes
+    """PEM-encoded certificate chain."""
+
+    key: bytes
+    """PEM-encoded private key."""
+
     uuid: str
     """
     Uniquely identifies the SiLA server. Needs to remain the same even after restarting the server.
     Follows the textual representation of UUIDs, e.g. "082bc5dc-18ae-4e17-b028-6115bbc6d21e".
     """
 
     name: str
@@ -68,17 +81,28 @@
             uuid=config.get("uuid", str(uuid.uuid4())),
             type=config.get("type", "ExampleServer"),
             name=config.get("name", "SiLA Server"),
             version=config.get("version", "0.1"),
             description=config.get("description", ""),
             vendor_url=config.get("vendor_url", "https://github.com/UniteLabs/driver"),
         )
-        self.host = config.get("host", "[::]")
+        self.host = config.get("host", "0.0.0.0")
         self.port = config.get("port", 0)
 
+        if config.get("tls", False):
+            cert = config.get("cert", None)
+            key = config.get("key", None)
+
+            if cert is None or key is None:
+                raise ValueError("When enabling TLS based server encryption, please provide both a cert and key file.")
+
+            self.certificate = (key, cert)
+        else:
+            self.certificate = None
+
         self.server = grpc.aio.server()
         self.running = False
         self.features: dict[identifiers.FullyQualifiedFeatureIdentifier, Feature] = {}
 
         self.command_executions: dict[str, commands.CommandExecution] = {}
 
     @property
@@ -90,15 +114,21 @@
 
     async def start(self):
         """Starts this Server."""
         if self.running:
             raise RuntimeError("Server is already running.")
 
         try:
-            self.port = self.server.add_insecure_port(f"{self.host}:{self.port}")
+            address = f"{self.host}:{self.port}"
+            if self.certificate:
+                credentials = grpc.ssl_server_credentials([self.certificate])
+                self.port = self.server.add_secure_port(address, credentials)
+            else:
+                self.port = self.server.add_insecure_port(address)
+
             await self.server.start()
             self.logger.info("Starting SiLA server on address '%s:%s'...", self.host, self.port)
             self.running = True
             await self.server.wait_for_termination()
         except asyncio.CancelledError:
             await self.stop()
```

### Comparing `unitelabs_sila-0.1.1/src/sila/server/unobservable_command.py` & `unitelabs_sila-0.1.2/src/sila/server/unobservable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/server/unobservable_property.py` & `unitelabs_sila-0.1.2/src/sila/server/unobservable_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/validators/display_name.py` & `unitelabs_sila-0.1.2/src/sila/validators/display_name.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/validators/domain.py` & `unitelabs_sila-0.1.2/src/sila/validators/domain.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/validators/identifier.py` & `unitelabs_sila-0.1.2/src/sila/validators/identifier.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/validators/uuid.py` & `unitelabs_sila-0.1.2/src/sila/validators/uuid.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/validators/validator.py` & `unitelabs_sila-0.1.2/src/sila/validators/validator.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/src/sila/validators/version.py` & `unitelabs_sila-0.1.2/src/sila/validators/version.py`

 * *Files identical despite different names*

### Comparing `unitelabs_sila-0.1.1/PKG-INFO` & `unitelabs_sila-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitelabs-sila
-Version: 0.1.1
+Version: 0.1.2
 Summary: An un-opinionated SiLA 2 library.
 Home-page: https://sila-standard.com
 License: MIT
 Keywords: SiLA 2,laboratory,automation,connectivity
 Author: UniteLabs AG
 Author-email: developers+sila@unitelabs.ch
 Requires-Python: >=3.9,<4.0
```

