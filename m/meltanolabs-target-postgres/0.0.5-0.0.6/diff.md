# Comparing `tmp/meltanolabs_target_postgres-0.0.5.tar.gz` & `tmp/meltanolabs_target_postgres-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_postgres-0.0.5.tar", max compression
+gzip compressed data, was "meltanolabs_target_postgres-0.0.6.tar", max compression
```

## Comparing `meltanolabs_target_postgres-0.0.5.tar` & `meltanolabs_target_postgres-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0     1068 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/LICENSE
--rw-r--r--   0        0        0     8242 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/README.md
--rw-r--r--   0        0        0     1750 2023-04-11 21:02:58.785164 meltanolabs_target_postgres-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/.gitignore
--rw-r--r--   0        0        0       21 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/__init__.py
--rw-r--r--   0        0        0     6548 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/connector.py
--rw-r--r--   0        0        0    11690 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/sinks.py
--rw-r--r--   0        0        0     6460 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/target.py
--rw-r--r--   0        0        0       38 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/__init__.py
--rw-r--r--   0        0        0     1681 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/activate_version_hard.singer
--rw-r--r--   0        0        0     1681 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/activate_version_soft.singer
--rw-r--r--   0        0        0      668 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/array_data.singer
--rw-r--r--   0        0        0      394 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/camelcase.singer
--rw-r--r--   0        0        0     1862 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/camelcase_complex_schema.singer
--rw-r--r--   0        0        0      722 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/duplicate_records.singer
--rw-r--r--   0        0        0     4275 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/encoded_strings.singer
--rw-r--r--   0        0        0      104 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/invalid_schema.singer
--rw-r--r--   0        0        0      362 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/large_int.singer
--rw-r--r--   0        0        0      607 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/missing_value.singer
--rw-r--r--   0        0        0     2129 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/multiple_state_messages.singer
--rw-r--r--   0        0        0      407 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/new_array_column.singer
--rw-r--r--   0        0        0      450 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/no_primary_keys.singer
--rw-r--r--   0        0        0      611 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/no_primary_keys_append.singer
--rw-r--r--   0        0        0      641 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/optional_attributes.singer
--rw-r--r--   0        0        0      378 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/record_before_schema.singer
--rw-r--r--   0        0        0      288 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/record_missing_key_property.singer
--rw-r--r--   0        0        0      318 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/record_missing_required_property.singer
--rw-r--r--   0        0        0    51890 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/reserved_keywords.singer
--rw-r--r--   0        0        0      892 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_no_properties.singer
--rw-r--r--   0        0        0     2197 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_updates.singer
--rw-r--r--   0        0        0      554 2023-04-11 21:02:36.693056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/special_chars_in_attributes.singer
--rw-r--r--   0        0        0  1859439 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_aapl.singer
--rw-r--r--   0        0        0    97655 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_countries.singer
--rw-r--r--   0        0        0     1851 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer
--rw-r--r--   0        0        0      357 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/test_activate_version_deletes_data_properly_2.singer
--rw-r--r--   0        0        0     1992 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_data.singer
--rw-r--r--   0        0        0     2323 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_upsert_data.singer
--rw-r--r--   0        0        0       15 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/.gitignore
--rw-r--r--   0        0        0      453 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/README.md
--rw-r--r--   0        0        0       15 2023-04-11 21:02:36.701056 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/__init__.py
--rw-r--r--   0        0        0   763998 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/AAPL.json
--rw-r--r--   0        0        0      352 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/README.md
--rw-r--r--   0        0        0      131 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/__main__.py
--rw-r--r--   0        0        0      654 2023-04-11 21:02:36.705057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/aapl.py
--rw-r--r--   0        0        0  1492450 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/fundamentals.json
--rw-r--r--   0        0        0       28 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/__init__.py
--rw-r--r--   0        0        0     2218 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_streams.py
--rw-r--r--   0        0        0      817 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_tap.py
--rw-r--r--   0        0        0      146 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/schemas/continents.json
--rw-r--r--   0        0        0    14720 2023-04-11 21:02:36.709057 meltanolabs_target_postgres-0.0.5/target_postgres/tests/test_standard_target.py
--rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 meltanolabs_target_postgres-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-14 20:47:32.349694 meltanolabs_target_postgres-0.0.6/LICENSE
+-rw-r--r--   0        0        0    10130 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/README.md
+-rw-r--r--   0        0        0     1765 2023-07-14 20:47:53.185944 meltanolabs_target_postgres-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/.gitignore
+-rw-r--r--   0        0        0       21 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/__init__.py
+-rw-r--r--   0        0        0    26885 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/connector.py
+-rw-r--r--   0        0        0    14118 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/sinks.py
+-rw-r--r--   0        0        0    13675 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/target.py
+-rw-r--r--   0        0        0       38 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/__init__.py
+-rw-r--r--   0        0        0      668 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/array_data.singer
+-rw-r--r--   0        0        0      394 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/camelcase.singer
+-rw-r--r--   0        0        0     1862 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/camelcase_complex_schema.singer
+-rw-r--r--   0        0        0     6910 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/commits.singer
+-rw-r--r--   0        0        0      722 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/duplicate_records.singer
+-rw-r--r--   0        0        0     4275 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/encoded_strings.singer
+-rw-r--r--   0        0        0      104 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/invalid_schema.singer
+-rw-r--r--   0        0        0      362 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/large_int.singer
+-rw-r--r--   0        0        0      607 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/missing_value.singer
+-rw-r--r--   0        0        0     2129 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/multiple_state_messages.singer
+-rw-r--r--   0        0        0      407 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/new_array_column.singer
+-rw-r--r--   0        0        0      641 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/optional_attributes.singer
+-rw-r--r--   0        0        0      378 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/record_before_schema.singer
+-rw-r--r--   0        0        0      288 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/record_missing_key_property.singer
+-rw-r--r--   0        0        0      318 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/record_missing_required_property.singer
+-rw-r--r--   0        0        0    51890 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/reserved_keywords.singer
+-rw-r--r--   0        0        0      892 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/schema_no_properties.singer
+-rw-r--r--   0        0        0     2197 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/schema_updates.singer
+-rw-r--r--   0        0        0      554 2023-07-14 20:47:32.353694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/special_chars_in_attributes.singer
+-rw-r--r--   0        0        0  1859439 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/tap_aapl.singer
+-rw-r--r--   0        0        0    97655 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/tap_countries.singer
+-rw-r--r--   0        0        0     1851 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer
+-rw-r--r--   0        0        0      357 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_activate_version_deletes_data_properly_2.singer
+-rw-r--r--   0        0        0     1681 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_activate_version_hard.singer
+-rw-r--r--   0        0        0     1681 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_activate_version_soft.singer
+-rw-r--r--   0        0        0      450 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_no_pk.singer
+-rw-r--r--   0        0        0      611 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_no_pk_append.singer
+-rw-r--r--   0        0        0      915 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/uppercase_stream_name_with_column_alter.singer
+-rw-r--r--   0        0        0     1992 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/user_location_data.singer
+-rw-r--r--   0        0        0     2323 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/user_location_upsert_data.singer
+-rw-r--r--   0        0        0       15 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/.gitignore
+-rw-r--r--   0        0        0      453 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/README.md
+-rw-r--r--   0        0        0       15 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/__init__.py
+-rw-r--r--   0        0        0   763998 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/AAPL.json
+-rw-r--r--   0        0        0      352 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/README.md
+-rw-r--r--   0        0        0      131 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/__main__.py
+-rw-r--r--   0        0        0      654 2023-07-14 20:47:32.361694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/aapl.py
+-rw-r--r--   0        0        0  1492450 2023-07-14 20:47:32.365694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/fundamentals.json
+-rw-r--r--   0        0        0       28 2023-07-14 20:47:32.365694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/sample_tap_countries/__init__.py
+-rw-r--r--   0        0        0     2218 2023-07-14 20:47:32.365694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/sample_tap_countries/countries_streams.py
+-rw-r--r--   0        0        0      817 2023-07-14 20:47:32.365694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/sample_tap_countries/countries_tap.py
+-rw-r--r--   0        0        0      146 2023-07-14 20:47:32.365694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/sample_tap_countries/schemas/continents.json
+-rw-r--r--   0        0        0    26392 2023-07-14 20:47:32.365694 meltanolabs_target_postgres-0.0.6/target_postgres/tests/test_standard_target.py
+-rw-r--r--   0        0        0    11304 1970-01-01 00:00:00.000000 meltanolabs_target_postgres-0.0.6/PKG-INFO
```

### Comparing `meltanolabs_target_postgres-0.0.5/LICENSE` & `meltanolabs_target_postgres-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/README.md` & `meltanolabs_target_postgres-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -10,43 +10,65 @@
 ## Capabilities
 
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
 ## Settings
-| Setting               | Required |       Default       | Description                                                                                                                                                                                                                                                            |
-| :-------------------- | :------: | :-----------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| host                  |  False   |        None         | Hostname for postgres instance. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                    |
-| port                  |  False   |        5432         | The port on which postgres is awaiting connection. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                 |
-| user                  |  False   |        None         | User name used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                    |
-| password              |  False   |        None         | Password used to authenticate. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                     |
-| database              |  False   |        None         | Database name. Note if sqlalchemy_url is set this will be ignored.                                                                                                                                                                                                     |
-| sqlalchemy_url        |  False   |        None         | SQLAlchemy connection string. This will override using host, user, password, port,dialect. Note that you must escape password special characters properly. See https://docs.sqlalchemy.org/en/20/core/engines.html#escaping-special-characters-such-as-signs-in-passwords |
-| dialect+driver        |  False   | postgresql+psycopg2 | Dialect+driver see https://docs.sqlalchemy.org/en/20/core/engines.html. Generally just leave this alone. Note if sqlalchemy_url is set this will be ignored.                                                                                                           |
-| default_target_schema |  False   |        None         | Postgres schema to send data to, example: tap-clickup                                                                                                                                                                                                                  |
-| hard_delete           |  False   |          0          | When activate version is sent from a tap this specefies if we should delete the records that don't match, or mark them with a date in the `_sdc_deleted_at` column.                                                                                                    |
-| add_record_metadata   |  False   |          1          | Note that this must be enabled for activate_version to work!This adds _sdc_extracted_at, _sdc_batched_at, and more to every table. See https://sdk.meltano.com/en/latest/implementation/record_metadata.html for more information.                                     |
-| stream_maps           |  False   |        None         | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html).                                                                                                                            |
-| stream_map_config     |  False   |        None         | User-defined config values to be used within map expressions.                                                                                                                                                                                                          |
-| flattening_enabled    |  False   |        None         | 'True' to enable schema flattening and automatically expand nested properties.                                                                                                                                                                                         |
-| flattening_max_depth  |  False   |        None         | The max depth to flatten schemas.                                                                                                                                                                                                                                      |
+| Setting                      | Required | Default | Description |
+|:-----------------------------|:--------:|:-------:|:------------|
+| host                         | False    | None    | Hostname for postgres instance. Note if sqlalchemy_url is set this will be ignored. |
+| port                         | False    |    5432 | The port on which postgres is awaiting connection. Note if sqlalchemy_url is set this will be ignored. |
+| user                         | False    | None    | User name used to authenticate. Note if sqlalchemy_url is set this will be ignored. |
+| password                     | False    | None    | Password used to authenticate. Note if sqlalchemy_url is set this will be ignored. |
+| database                     | False    | None    | Database name. Note if sqlalchemy_url is set this will be ignored. |
+| sqlalchemy_url               | False    | None    | SQLAlchemy connection string. This will override using host, user, password, port, dialect, and all ssl settings. Note that you must escape password special characters properly. See https://docs.sqlalchemy.org/en/20/core/engines.html#escaping-special-characters-such-as-signs-in-passwords |
+| dialect+driver               | False    | postgresql+psycopg2 | Dialect+driver see https://docs.sqlalchemy.org/en/20/core/engines.html. Generally just leave this alone. Note if sqlalchemy_url is set this will be ignored. |
+| default_target_schema        | False    | None    | Postgres schema to send data to, example: tap-clickup |
+| hard_delete                  | False    |       0 | When activate version is sent from a tap this specefies if we should delete the records that don't match, or mark them with a date in the `_sdc_deleted_at` column. |
+| add_record_metadata          | False    |       1 | Note that this must be enabled for activate_version to work!This adds _sdc_extracted_at, _sdc_batched_at, and more to every table. See https://sdk.meltano.com/en/latest/implementation/record_metadata.html for more information. |
+| ssh_tunnel                   | False    | None    | SSH Tunnel Configuration, this is a json object |
+| ssh_tunnel.enable   | True (if ssh_tunnel set) | False   | Enable an ssh tunnel (also known as bastion host), see the other ssh_tunnel.* properties for more details.
+| ssh_tunnel.host | True (if ssh_tunnel set) | False   | Host of the bastion host, this is the host we'll connect to via ssh
+| ssh_tunnel.username | True (if ssh_tunnel set) | False   |Username to connect to bastion host
+| ssh_tunnel.port | True (if ssh_tunnel set) | 22 | Port to connect to bastion host
+| ssh_tunnel.private_key | True (if ssh_tunnel set) | None | Private Key for authentication to the bastion host
+| ssh_tunnel.private_key_password | False | None | Private Key Password, leave None if no password is set
+| ssl_enable                   | False    |       0 | Whether or not to use ssl to verify the server's identity. Use ssl_certificate_authority and ssl_mode for further customization. To use a client certificate to authenticate yourself to the server, use ssl_client_certificate_enable instead. Note if sqlalchemy_url is set this will be ignored. |
+| ssl_client_certificate_enable| False    |       0 | Whether or not to provide client-side certificates as a method of authentication to the server. Use ssl_client_certificate and ssl_client_private_key for further customization. To use SSL to verify the server's identity, use ssl_enable instead. Note if sqlalchemy_url is set this will be ignored. |
+| ssl_mode                     | False    | verify-full | SSL Protection method, see [postgres documentation](https://www.postgresql.org/docs/current/libpq-ssl.html#LIBPQ-SSL-PROTECTION) for more information. Must be one of disable, allow, prefer, require, verify-ca, or verify-full. Note if sqlalchemy_url is set this will be ignored. |
+| ssl_certificate_authority    | False    | ~/.postgresql/root.crl | The certificate authority that should be used to verify the server's identity. Can be provided either as the certificate itself (in .env) or as a filepath to the certificate. Note if sqlalchemy_url is set this will be ignored. |
+| ssl_client_certificate       | False    | ~/.postgresql/postgresql.crt | The certificate that should be used to verify your identity to the server. Can be provided either as the certificate itself (in .env) or as a filepath to the certificate. Note if sqlalchemy_url is set this will be ignored. |
+| ssl_client_private_key       | False    | ~/.postgresql/postgresql.key | The private key for the certificate you provided. Can be provided either as the certificate itself (in .env) or as a filepath to the certificate. Note if sqlalchemy_url is set this will be ignored. |
+| ssl_storage_directory        | False    | .secrets | The folder in which to store SSL certificates provided as raw values. When a certificate/key is provided as a raw value instead of as a filepath, it must be written to a file before it can be used. This configuration option determines where that file is created. |
+| stream_maps                  | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
+| stream_map_config            | False    | None    | User-defined config values to be used within map expressions. |
+| flattening_enabled           | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
+| flattening_max_depth         | False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-postgres --about`
 
 ## Installation
 
 - [ ] `Developer TODO:` Come back to this re [#5](https://github.com/MeltanoLabs/target-postgres/issues/5)
 
 ```bash
 pipx install -e .
 ```
 
 ## Configuration
 
+### An Explanation of Various SSL Configuration Options
+
+There are two distinct processes which both fall under the banner of SSL. One process occurs when the client wishes to ensure the identity of the server, and is the more common reason that SSL is used. Another is when the server wishes to ensure the identity of the client, for authentication/authorization purposes.
+
+If your server is set up with a certificate and private key, and you wish to check their certificate against a root certificate which you posess, use `ssl_enable`. You may then further customize this process using the `ssl_certificate_authority` and `ssl_mode` settings. See the [documentation](https://www.postgresql.org/docs/current/libpq-ssl.html#LIBQ-SSL-CERTIFICATES) for further details.
+
+If your server is set up with a root certificate, and you wish to provide a certificate to the server to verify your identity, use `ssl_client_certificate_enable`. You may then further customize this process using the `ssl_client_certificate` and `ssl_client_private_key` settings. See the [documentation](https://www.postgresql.org/docs/current/libpq-ssl.html#LIBPQ-SSL-CLIENTCERT) for further details.
+
 ### Configure using environment variables
 
 This Singer target will automatically import any environment variables within the working directory's
 `.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
 environment variable is set either in the terminal context or in the `.env` file.
 
 ### Source Authentication and Authorization
@@ -66,14 +88,18 @@
 target-postgres --version
 target-postgres --help
 # Test using the "Carbon Intensity" sample:
 pipx install git+https://gitlab.com/meltano/tap-carbon-intensity
 tap-carbon-intensity | target-postgres --config /path/to/target-postgres-config.json
 ```
 
+### Using Docker Compose
+
+`docker-compose.yml` provides the commands to create two empty sample databases using [Docker](https://docs.docker.com/engine/install/). These can be a starting point to create your own database running in Docker, or can be used to run the tap's [built-in tests](#create-and-run-tests).
+
 ## Developer Resources
 
 ### Initialize your Development Environment
 
 ```bash
 pipx install poetry
 poetry install
```

### Comparing `meltanolabs_target_postgres-0.0.5/pyproject.toml` & `meltanolabs_target_postgres-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-postgres"
-version = "0.0.5"
+version = "0.0.6"
 description = "`target-postgres` is a Singer target for Postgres, built with the Meltano SDK for Singer Targets."
 authors = ["Meltano Team and Contributors"]
 maintainers = ["Meltano Team and Contributors"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://meltano.com"
 repository = "https://github.com/meltanolabs/target-postgres"
@@ -29,19 +29,20 @@
 packages = [
     { include = "target_postgres" }
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = ">=0.17,<0.20"
-psycopg2-binary = "2.9.5"
+singer-sdk = "^0.28.0"
+psycopg2-binary = "2.9.6"
+sshtunnel = "0.4.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
+pytest = "^7.3.2"
 tox = "^3.24.4"
 flake8 = "^5.0.4"
 flake8-docstrings = "^1.7.0"
 black = "23.1.0"
 mypy = "^1.0"
 isort = "^5.11.5"
 remote-pdb="2.1.0"
```

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/.gitignore` & `meltanolabs_target_postgres-0.0.6/target_postgres/.gitignore`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/sinks.py` & `meltanolabs_target_postgres-0.0.6/target_postgres/sinks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,156 +1,125 @@
 """Postgres target sink class, which handles writing streams."""
+
 import uuid
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import sqlalchemy
 from pendulum import now
 from singer_sdk.sinks import SQLSink
-from sqlalchemy import Column, MetaData, Table, insert
+from sqlalchemy import Column, MetaData, Table, insert, select, update
 from sqlalchemy.sql import Executable
 from sqlalchemy.sql.expression import bindparam
 
 from target_postgres.connector import PostgresConnector
 
 
 class PostgresSink(SQLSink):
     """Postgres target sink class."""
 
     connector_class = PostgresConnector
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, target, *args, **kwargs):
         """Initialize SQL Sink. See super class for more details."""
-        super().__init__(*args, **kwargs)
+        connector = PostgresConnector(config=dict(target.config))
+        super().__init__(target=target, connector=connector, *args, **kwargs)
         self.temp_table_name = self.generate_temp_table_name()
 
+    @property
+    def append_only(self) -> bool:
+        """Return True if the target is append only."""
+        return self._append_only
+
+    @append_only.setter
+    def append_only(self, value: bool) -> None:
+        """Set the append_only attribute."""
+        self._append_only = value
+
     def setup(self) -> None:
         """Set up Sink.
 
         This method is called on Sink creation, and creates the required Schema and
         Table entities in the target database.
         """
         if self.key_properties is None or self.key_properties == []:
-            raise ValueError(
-                "key_properties must be set. See"
-                "https://github.com/MeltanoLabs/target-postgres/issues/54"
-                "for more information."
-            )
+            self.append_only = True
+        else:
+            self.append_only = False
         if self.schema_name:
             self.connector.prepare_schema(self.schema_name)
-        self.connector.prepare_table(
-            full_table_name=self.full_table_name,
-            schema=self.schema,
-            primary_keys=self.key_properties,
-            as_temp_table=False,
-        )
+        with self.connector._connect() as connection:
+            self.connector.prepare_table(
+                full_table_name=self.full_table_name,
+                schema=self.schema,
+                primary_keys=self.key_properties,
+                connection=connection,
+                as_temp_table=False,
+            )
 
     def process_batch(self, context: dict) -> None:
         """Process a batch with the given batch context.
 
         Writes a batch to the SQL target. Developers may override this method
         in order to provide a more efficient upload/upsert process.
 
         Args:
             context: Stream partition or context dictionary.
         """
-        # First we need to be sure the main table is already created
-        self.connector.prepare_table(
-            full_table_name=self.full_table_name,
-            schema=self.schema,
-            primary_keys=self.key_properties,
-            as_temp_table=False,
-        )
-        # Create a temp table (Creates from the table above)
-        self.connector.create_temp_table_from_table(
-            from_table_name=self.full_table_name, temp_table_name=self.temp_table_name
-        )
-        # Insert into temp table
-        self.bulk_insert_records(
-            full_table_name=self.temp_table_name,
-            schema=self.schema,
-            primary_keys=self.key_properties,
-            records=context["records"],
-        )
-        # Merge data from Temp table to main table
-        self.merge_upsert_from_table(
-            from_table_name=self.temp_table_name,
-            to_table_name=self.full_table_name,
-            schema=self.schema,
-            join_keys=self.key_properties,
-        )
-        # Drop temp table
-        self.connector.drop_table(self.temp_table_name)
+        # Use one connection so we do this all in a single transaction
+        with self.connector._connect() as connection:
+            # Check structure of table
+            table: sqlalchemy.Table = self.connector.prepare_table(
+                full_table_name=self.full_table_name,
+                schema=self.schema,
+                primary_keys=self.key_properties,
+                as_temp_table=False,
+                connection=connection,
+            )
+            # Create a temp table (Creates from the table above)
+            temp_table: sqlalchemy.Table = self.connector.copy_table_structure(
+                full_table_name=self.temp_table_name,
+                from_table=table,
+                as_temp_table=True,
+                connection=connection,
+            )
+            # Insert into temp table
+            self.bulk_insert_records(
+                table=temp_table,
+                schema=self.schema,
+                primary_keys=self.key_properties,
+                records=context["records"],
+                connection=connection,
+            )
+            # Merge data from Temp table to main table
+            self.upsert(
+                from_table=temp_table,
+                to_table=table,
+                schema=self.schema,
+                join_keys=self.key_properties,
+                connection=connection,
+            )
+            # Drop temp table
+            self.connector.drop_table(table=temp_table, connection=connection)
 
     def generate_temp_table_name(self):
         """Uuid temp table name."""
-        # Table name makes debugging easier when data cannot be written to the
-        # temp table for some reason
-        return f"temp_{self.table_name}_{str(uuid.uuid4()).replace('-','_')}"
-
-    def merge_upsert_from_table(
-        self,
-        from_table_name: str,
-        to_table_name: str,
-        schema: dict,
-        join_keys: List[str],
-    ) -> Optional[int]:
-        """Merge upsert data from one table to another.
-
-        Args:
-            from_table_name: The source table name.
-            to_table_name: The destination table name.
-            join_keys: The merge upsert keys, or `None` to append.
-            schema: Singer Schema message.
-
-        Return:
-            The number of records copied, if detectable, or `None` if the API does not
-            report number of records affected/inserted.
-
-        """
-        # TODO think about sql injeciton,
-        # issue here https://github.com/MeltanoLabs/target-postgres/issues/22
-
-        # INSERT
-        join_condition = " and ".join(
-            [f'temp."{key}" = target."{key}"' for key in join_keys]
-        )
-        where_condition = " and ".join([f'target."{key}" is null' for key in join_keys])
-
-        insert_sql = f"""
-        INSERT INTO {to_table_name}
-        SELECT
-        temp.*
-        FROM {from_table_name} AS temp
-        LEFT JOIN {to_table_name} AS target ON {join_condition}
-        WHERE {where_condition}
-        """
-        self.connection.execute(insert_sql)
-
-        # UPDATE
-        columns = ", ".join(
-            [
-                f'"{column_name}"=temp."{column_name}"'
-                for column_name in self.schema["properties"].keys()
-            ]
-        )
-        where_condition = join_condition
-        update_sql = f"""
-        UPDATE {to_table_name} AS target
-        SET {columns}
-        FROM {from_table_name} AS temp
-        WHERE {where_condition}
-        """
-        self.connection.execute(update_sql)
+        # sqlalchemy.exc.IdentifierError: Identifier
+        # 'temp_test_optional_attributes_388470e9_fbd0_47b7_a52f_d32a2ee3f5f6'
+        # exceeds maximum length of 63 characters
+        # Is hit if we have a long table name, there is no limit on Temporary tables
+        # in postgres, used a guid just in case we are using the same session
+        return f"{str(uuid.uuid4()).replace('-','_')}"
 
     def bulk_insert_records(
         self,
-        full_table_name: str,
+        table: sqlalchemy.Table,
         schema: dict,
         records: Iterable[Dict[str, Any]],
         primary_keys: List[str],
+        connection: sqlalchemy.engine.Connection,
     ) -> Optional[int]:
         """Bulk insert records to an existing destination table.
 
         The default implementation uses a generic SQLAlchemy bulk insert operation.
         This method may optionally be overridden by developers in order to provide
         faster, native bulk uploads.
 
@@ -161,38 +130,118 @@
             records: the input records.
 
         Returns:
             True if table exists, False if not, None if unsure or undetectable.
         """
         columns = self.column_representation(schema)
         insert = self.generate_insert_statement(
-            full_table_name,
+            table.name,
             columns,
         )
         self.logger.info("Inserting with SQL: %s", insert)
         # Only one record per PK, we want to take the last one
-        insert_records: Dict[str, Dict] = {}  # pk : record
-        for record in records:
-            insert_record = {}
-            for column in columns:
-                insert_record[column.name] = record.get(column.name)
+        data_to_insert: List[Dict[str, Any]] = []
+
+        if self.append_only is False:
+            insert_records: Dict[str, Dict] = {}  # pk : record
             try:
-                primary_key_value = "".join([str(record[key]) for key in primary_keys])
+                for record in records:
+                    insert_record = {}
+                    for column in columns:
+                        insert_record[column.name] = record.get(column.name)
+                    primary_key_value = "".join(
+                        [str(record[key]) for key in primary_keys]
+                    )
+                    insert_records[primary_key_value] = insert_record
             except KeyError:
                 raise RuntimeError(
                     "Primary key not found in record. "
-                    f"full_table_name: {full_table_name}. "
-                    f"schema: {schema}.  "
+                    f"full_table_name: {table.name}. "
+                    f"schema: {table.schema}.  "
                     f"primary_keys: {primary_keys}."
                 )
-            insert_records[primary_key_value] = insert_record
-
-        self.connector.connection.execute(insert, list(insert_records.values()))
+            data_to_insert = list(insert_records.values())
+        else:
+            for record in records:
+                insert_record = {}
+                for column in columns:
+                    insert_record[column.name] = record.get(column.name)
+                data_to_insert.append(insert_record)
+        connection.execute(insert, data_to_insert)
         return True
 
+    def upsert(
+        self,
+        from_table: sqlalchemy.Table,
+        to_table: sqlalchemy.Table,
+        schema: dict,
+        join_keys: List[Column],
+        connection: sqlalchemy.engine.Connection,
+    ) -> Optional[int]:
+        """Merge upsert data from one table to another.
+
+        Args:
+            from_table_name: The source table name.
+            to_table_name: The destination table name.
+            join_keys: The merge upsert keys, or `None` to append.
+            schema: Singer Schema message.
+
+        Return:
+            The number of records copied, if detectable, or `None` if the API does not
+            report number of records affected/inserted.
+
+        """
+        if self.append_only is True:
+            # Insert
+            select_stmt = select(from_table.columns).select_from(from_table)
+            insert_stmt = to_table.insert().from_select(
+                names=from_table.columns, select=select_stmt
+            )
+            connection.execute(insert_stmt)
+        else:
+            join_predicates = []
+            for key in join_keys:
+                from_table_key: sqlalchemy.Column = from_table.columns[key]
+                to_table_key: sqlalchemy.Column = to_table.columns[key]
+                join_predicates.append(from_table_key == to_table_key)
+
+            join_condition = sqlalchemy.and_(*join_predicates)
+
+            where_predicates = []
+            for key in join_keys:
+                to_table_key: sqlalchemy.Column = to_table.columns[key]
+                where_predicates.append(to_table_key.is_(None))
+            where_condition = sqlalchemy.and_(*where_predicates)
+
+            select_stmt = (
+                select(from_table.columns)
+                .select_from(from_table.outerjoin(to_table, join_condition))
+                .where(where_condition)
+            )
+            insert_stmt = insert(to_table).from_select(
+                names=from_table.columns, select=select_stmt
+            )
+
+            connection.execute(insert_stmt)
+
+            # Update
+            where_condition = join_condition
+            update_columns = {}
+            for column_name in self.schema["properties"].keys():
+                from_table_column: sqlalchemy.Column = from_table.columns[column_name]
+                to_table_column: sqlalchemy.Column = to_table.columns[column_name]
+                update_columns[from_table_column] = to_table_column
+
+            update_stmt = (
+                update(from_table).where(where_condition).values(update_columns)
+            )
+            connection.execute(update_stmt)
+
+        return None
+
     def column_representation(
         self,
         schema: dict,
     ) -> List[Column]:
         """Return a sqlalchemy table representation for the current schema."""
         columns: list[Column] = []
         for property_name, property_jsonschema in schema["properties"].items():
@@ -314,8 +363,9 @@
             f"OR {self.version_column_name} IS NULL \n"
             f"  AND {self.soft_delete_column_name} IS NULL\n"
         )
         query = query.bindparams(
             bindparam("deletedate", value=deleted_at, type_=datetime_type),
             bindparam("version", value=new_version, type_=integer_type),
         )
-        self.connector.connection.execute(query)
+        with self.connector._connect() as connection:
+            connection.execute(query)
```

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/activate_version_hard.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_activate_version_hard.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/activate_version_soft.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_activate_version_soft.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/array_data.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/array_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/camelcase_complex_schema.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/camelcase_complex_schema.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/duplicate_records.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/duplicate_records.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/encoded_strings.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/encoded_strings.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/missing_value.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/missing_value.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/multiple_state_messages.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/multiple_state_messages.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/no_primary_keys_append.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_no_pk_append.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/optional_attributes.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/optional_attributes.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/reserved_keywords.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/reserved_keywords.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_no_properties.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/schema_no_properties.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/schema_updates.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/schema_updates.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/special_chars_in_attributes.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/special_chars_in_attributes.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_aapl.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/tap_aapl.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/tap_countries.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/tap_countries.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_data.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/user_location_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/data_files/user_location_upsert_data.singer` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/data_files/user_location_upsert_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/AAPL.json` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/AAPL.json`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/aapl.py` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/aapl.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/aapl/fundamentals.json` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/aapl/fundamentals.json`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_streams.py` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/sample_tap_countries/countries_streams.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.5/target_postgres/tests/samples/sample_tap_countries/countries_tap.py` & `meltanolabs_target_postgres-0.0.6/target_postgres/tests/samples/sample_tap_countries/countries_tap.py`

 * *Files identical despite different names*

