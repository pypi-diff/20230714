# Comparing `tmp/whylogs-1.2.3.tar.gz` & `tmp/whylogs-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.2.3.tar", max compression
+gzip compressed data, was "whylogs-1.2.4.tar", max compression
```

## Comparing `whylogs-1.2.3.tar` & `whylogs-1.2.4.tar`

### file list

```diff
@@ -1,216 +1,216 @@
--rw-r--r--   0        0        0     3166 2023-07-12 19:52:30.695318 whylogs-1.2.3/DESCRIPTION.md
--rw-r--r--   0        0        0     5846 2023-07-12 19:52:56.935751 whylogs-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/annotations.py
--rw-r--r--   0        0        0      120 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0     8157 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
--rw-r--r--   0        0        0      468 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
--rw-r--r--   0        0        0     2119 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
--rw-r--r--   0        0        0    15693 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
--rw-r--r--   0        0        0     3964 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
--rw-r--r--   0        0        0     4770 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    19765 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9550 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     6333 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6168 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7663 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0     7497 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      329 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3813 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0    10646 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0      666 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      947 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1169 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2084 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3408 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    40899 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1217 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0     1090 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3391 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2023-07-12 19:52:30.739318 whylogs-1.2.3/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30671 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11486 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4120 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/errors.py
--rw-r--r--   0        0        0     2560 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     1740 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     7615 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0     8976 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14489 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2023-07-12 19:53:00.371806 whylogs-1.2.3/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2023-07-12 19:52:59.251788 whylogs-1.2.3/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2023-07-12 19:52:59.251788 whylogs-1.2.3/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2023-07-12 19:52:59.251788 whylogs-1.2.3/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2023-07-12 19:53:00.515808 whylogs-1.2.3/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2023-07-12 19:52:59.251788 whylogs-1.2.3/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2023-07-12 19:52:59.151786 whylogs-1.2.3/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2023-07-12 19:52:59.151786 whylogs-1.2.3/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/relations.py
--rw-r--r--   0        0        0    11101 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10029 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2087 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     1602 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      210 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4760 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0      508 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    17663 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     8747 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    13776 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0     8861 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1554 2023-07-12 19:52:30.743318 whylogs-1.2.3/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    10031 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15367 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/migration/converters.py
--rw-r--r--   0        0        0     6959 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    21751 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2023-07-12 19:52:30.747319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2023-07-12 19:52:30.751319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2023-07-12 19:52:30.755319 whylogs-1.2.3/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2023-07-12 19:52:30.759319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    21376 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1060 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2023-07-12 19:52:30.763319 whylogs-1.2.3/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 whylogs-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3166 2023-07-14 14:40:50.259786 whylogs-1.2.4/DESCRIPTION.md
+-rw-r--r--   0        0        0     5846 2023-07-14 14:41:16.932217 whylogs-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1801 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      120 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0     8157 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
+-rw-r--r--   0        0        0     2119 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
+-rw-r--r--   0        0        0    15693 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
+-rw-r--r--   0        0        0     3964 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
+-rw-r--r--   0        0        0     4770 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    19765 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9550 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     6333 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6168 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7663 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0     7497 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      329 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3813 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0    10646 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0      666 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      947 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     2726 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     1169 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2084 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     3408 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    40899 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0     1217 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0     1090 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3391 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30671 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11486 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4120 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/errors.py
+-rw-r--r--   0        0        0     2560 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     1740 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0     7615 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0     8976 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14489 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2023-07-14 14:41:20.464272 whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2023-07-14 14:41:20.612274 whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2023-07-14 14:41:19.076251 whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2023-07-14 14:41:19.076251 whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11101 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10029 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2087 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     1602 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      210 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4760 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0      508 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    17663 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     8747 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    13776 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0     8861 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1554 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    10031 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15367 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     6959 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    21751 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2502 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2023-07-14 14:40:50.327787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2023-07-14 14:40:50.327787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    21376 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1060 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 whylogs-1.2.4/PKG-INFO
```

### Comparing `whylogs-1.2.3/DESCRIPTION.md` & `whylogs-1.2.4/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/pyproject.toml` & `whylogs-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.2.3"
+version = "1.2.4"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
```

### Comparing `whylogs-1.2.3/whylogs/__init__.py` & `whylogs-1.2.4/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/annotations.py` & `whylogs-1.2.4/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/fugue/profiler.py` & `whylogs-1.2.4/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/fugue/registry.py` & `whylogs-1.2.4/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/__init__.py` & `whylogs-1.2.4/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py` & `whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py` & `whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py` & `whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/logger.py` & `whylogs-1.2.4/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/result_set.py` & `whylogs-1.2.4/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/rolling.py` & `whylogs-1.2.4/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/segment_cache.py` & `whylogs-1.2.4/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/segment_processing.py` & `whylogs-1.2.4/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/logger/transient.py` & `whylogs-1.2.4/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.2.4/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.2.4/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/reader/local.py` & `whylogs-1.2.4/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/reader/reader.py` & `whylogs-1.2.4/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/reader/s3.py` & `whylogs-1.2.4/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/store/local_store.py` & `whylogs-1.2.4/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/store/profile_store.py` & `whylogs-1.2.4/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/store/query.py` & `whylogs-1.2.4/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/store/sqlite_store.py` & `whylogs-1.2.4/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/usage_stats/__init__.py` & `whylogs-1.2.4/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/whylabs/session/config.py` & `whylogs-1.2.4/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.2.4/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.2.4/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.2.4/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/writer/__init__.py` & `whylogs-1.2.4/whylogs/api/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/writer/gcs.py` & `whylogs-1.2.4/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/writer/local.py` & `whylogs-1.2.4/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/writer/mlflow.py` & `whylogs-1.2.4/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/writer/s3.py` & `whylogs-1.2.4/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/api/writer/whylabs.py` & `whylogs-1.2.4/whylogs/api/writer/whylabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 
 def _validate_api_key(api_key: Optional[str]) -> str:
     if api_key is None:
         raise ValueError("Missing API key. Set it via WHYLABS_API_KEY environment variable or as an api_key option")
     if len(api_key) < 12:
         raise ValueError("API key too short")
-    if len(api_key) > 64:
+    if len(api_key) > 80:
         raise ValueError("API key too long")
     if api_key[10] != ".":
         raise ValueError("Invalid format. Expecting a dot at an index 10")
     return api_key[:10]
 
 
 class KeyRefresher(abc.ABC):
```

### Comparing `whylogs-1.2.3/whylogs/api/writer/writer.py` & `whylogs-1.2.4/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/__init__.py` & `whylogs-1.2.4/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/column_profile.py` & `whylogs-1.2.4/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/configs.py` & `whylogs-1.2.4/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.2.4/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.2.4/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/dataset_profile.py` & `whylogs-1.2.4/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/datatypes.py` & `whylogs-1.2.4/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/errors.py` & `whylogs-1.2.4/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/feature_weights.py` & `whylogs-1.2.4/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/input_resolver.py` & `whylogs-1.2.4/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metric_getters.py` & `whylogs-1.2.4/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/__init__.py` & `whylogs-1.2.4/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/aggregators.py` & `whylogs-1.2.4/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/column_metrics.py` & `whylogs-1.2.4/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/compound_metric.py` & `whylogs-1.2.4/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.2.4/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/decorators.py` & `whylogs-1.2.4/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/deserializers.py` & `whylogs-1.2.4/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/maths.py` & `whylogs-1.2.4/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/metric_components.py` & `whylogs-1.2.4/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/metrics.py` & `whylogs-1.2.4/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/multimetric.py` & `whylogs-1.2.4/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/serializers.py` & `whylogs-1.2.4/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/metrics/unicode_range.py` & `whylogs-1.2.4/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.2.4/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.2.4/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.2.4/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/predicate_parser.py` & `whylogs-1.2.4/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/preprocessing.py` & `whylogs-1.2.4/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/relations.py` & `whylogs-1.2.4/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/resolvers.py` & `whylogs-1.2.4/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/schema.py` & `whylogs-1.2.4/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/segmentation_partition.py` & `whylogs-1.2.4/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/specialized_resolvers.py` & `whylogs-1.2.4/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/stubs.py` & `whylogs-1.2.4/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.2.4/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/utils/stats_calculations.py` & `whylogs-1.2.4/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/utils/utils.py` & `whylogs-1.2.4/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/validators/condition_validator.py` & `whylogs-1.2.4/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/view/column_profile_view.py` & `whylogs-1.2.4/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.2.4/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.2.4/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/base.py` & `whylogs-1.2.4/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/configs.py` & `whylogs-1.2.4/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.2.4/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/descr/employee.rst` & `whylogs-1.2.4/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/descr/weather.rst` & `whylogs-1.2.4/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/ecommerce.py` & `whylogs-1.2.4/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/employee.py` & `whylogs-1.2.4/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/utils.py` & `whylogs-1.2.4/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/datasets/weather.py` & `whylogs-1.2.4/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.2.4/whylogs/experimental/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.2.4/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.2.4/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.2.4/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.2.4/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.2.4/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.2.4/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.2.4/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.2.4/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/core/udf_schema.py` & `whylogs-1.2.4/whylogs/experimental/core/udf_schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.2.4/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.2.4/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.2.4/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.2.4/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.2.4/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.2.4/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/extras/image_metric.py` & `whylogs-1.2.4/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/migration/converters.py` & `whylogs-1.2.4/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/migration/uncompound.py` & `whylogs-1.2.4/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.2.4/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/drift/configs.py` & `whylogs-1.2.4/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/enums/enums.py` & `whylogs-1.2.4/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.2.4/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.2.4/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.2.4/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.2.4/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.2.4/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.2.4/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.2.4/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/js/d3.min.js` & `whylogs-1.2.4/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/js/handlebars.js` & `whylogs-1.2.4/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.2.4/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.2.4/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/html/templates/index.html` & `whylogs-1.2.4/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.2.4/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.2.4/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.2.4/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.2.4/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.2.4/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.2.4/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.2.4/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.2.4/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.3/PKG-INFO` & `whylogs-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.2.3
+Version: 1.2.4
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: whylogs Version: 1.2.3 Summary: Profile and monitor
+Metadata-Version: 2.1 Name: whylogs Version: 1.2.4 Summary: Profile and monitor
 your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai License:
 Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai Requires-Python:
 >=3.7.1,<4 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: datasets
```

