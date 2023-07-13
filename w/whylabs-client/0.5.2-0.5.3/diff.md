# Comparing `tmp/whylabs-client-0.5.2.tar.gz` & `tmp/whylabs-client-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.5.2.tar", last modified: Wed Jun 28 23:40:34 2023, max compression
+gzip compressed data, was "whylabs-client-0.5.3.tar", last modified: Thu Jul 13 22:40:04 2023, max compression
```

## Comparing `whylabs-client-0.5.2.tar` & `whylabs-client-0.5.3.tar`

### file list

```diff
@@ -1,161 +1,167 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:40:34.907048 whylabs-client-0.5.2/
--rw-r--r--   0 root         (0) root         (0)     3400 2023-06-28 23:40:34.909048 whylabs-client-0.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    24832 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-28 23:40:34.909048 whylabs-client-0.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-06-28 23:40:34.000000 whylabs-client-0.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:40:34.880048 whylabs-client-0.5.2/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:40:34.883048 whylabs-client-0.5.2/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    34743 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20727 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    67177 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52337 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    57772 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    29965 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37579 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:40:34.884048 whylabs-client-0.5.2/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17084 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:40:34.907048 whylabs-client-0.5.2/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12005 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11342 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/batch_log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11655 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/batch_log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12443 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12228 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/create_reference_profile_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12113 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/create_reference_profile_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11207 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13099 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/databricks_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dataset_request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/datatype_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/distribution_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_clusters_auto_scale_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13257 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_clusters_aws_attributes_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11739 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_clusters_aws_availability_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11804 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12362 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_clusters_s3_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11745 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_ebs_volume_type_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_cron_schedule_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11934 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_data_security_mode_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11969 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_job_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12404 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_job_email_notifications_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    16133 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_job_settings_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    16932 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_new_cluster_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11603 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_notebook_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11707 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_spark_jar_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_spark_python_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11293 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/dto_jobs_spark_submit_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12313 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12718 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/entity_search_result.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11507 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11411 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11431 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11485 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11379 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_monitor_config_v2_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/list_jobs_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11289 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/list_jobs_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11502 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11858 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11441 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12111 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11756 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12260 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/metric_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11120 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/missing_recent_data_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11132 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/missing_recent_profiles_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/missing_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    12569 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12351 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/monitor_request_reference.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/monitor_request_reference_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13005 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/notification_relationship_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11242 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/notification_relationship_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11982 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14425 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13737 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12319 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/provided_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11680 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/provision_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11657 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/provision_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12885 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11188 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/refresh_access_token_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11444 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/refresh_connection_by_org_id_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11586 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/refresh_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13668 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/register_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11112 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/register_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13372 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/request_feature_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15325 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11922 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/run_job_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11089 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/run_job_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11471 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11447 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/search_index_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11787 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/search_index_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/search_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/seasonal_arima_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11615 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/segment_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11948 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11760 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11610 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11917 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/unique_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/update_connection_changes.py
--rw-rw-rw-   0 root         (0) root         (0)    11816 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/update_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    13667 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model/why_logs_metric.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:40:34.907048 whylabs-client-0.5.2/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)    10508 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2023-06-28 23:40:24.000000 whylabs-client-0.5.2/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 23:40:34.882048 whylabs-client-0.5.2/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3400 2023-06-28 23:40:34.000000 whylabs-client-0.5.2/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7052 2023-06-28 23:40:34.000000 whylabs-client-0.5.2/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 23:40:34.000000 whylabs-client-0.5.2/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 23:40:34.000000 whylabs-client-0.5.2/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-28 23:40:34.000000 whylabs-client-0.5.2/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 22:40:04.477995 whylabs-client-0.5.3/
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-07-13 22:40:04.477995 whylabs-client-0.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    25770 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-13 22:40:04.477995 whylabs-client-0.5.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-07-13 22:40:03.000000 whylabs-client-0.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 22:40:04.451996 whylabs-client-0.5.3/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 22:40:04.454996 whylabs-client-0.5.3/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    34743 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    17246 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20727 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    67177 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52337 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    57772 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35435 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37579 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 22:40:04.454996 whylabs-client-0.5.3/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17084 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 22:40:04.476995 whylabs-client-0.5.3/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11353 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/admin_report_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11315 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/admin_report_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12005 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/batch_log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11655 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/batch_log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12443 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11959 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/create_dataset_profile_upload_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12228 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/create_reference_profile_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12113 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/create_reference_profile_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11207 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13099 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/databricks_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dataset_request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/datatype_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/distribution_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_clusters_auto_scale_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13257 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_clusters_aws_attributes_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11739 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_clusters_aws_availability_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11804 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_clusters_s3_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11745 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_ebs_volume_type_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_cron_schedule_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11934 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_data_security_mode_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11969 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_job_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_job_email_notifications_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16133 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_job_settings_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_new_cluster_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11603 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_notebook_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11707 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_spark_jar_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_spark_python_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11293 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/dto_jobs_spark_submit_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12313 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12718 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/entity_search_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11507 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11411 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11379 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_monitor_config_v2_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11451 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_profile_observatory_link_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11434 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_profile_observatory_link_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/list_jobs_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11289 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/list_jobs_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11502 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11858 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11441 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12111 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11756 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11120 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/missing_recent_data_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11132 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/missing_recent_profiles_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/missing_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12569 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12351 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/monitor_request_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/monitor_request_reference_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13005 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/notification_relationship_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11242 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/notification_relationship_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11982 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14425 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13737 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12319 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/provided_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11680 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/provision_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/provision_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12885 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11188 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/refresh_access_token_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11444 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/refresh_connection_by_org_id_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11586 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/refresh_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13668 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/register_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11112 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/register_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13372 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/request_feature_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15325 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11922 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/run_job_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11089 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/run_job_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11471 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11447 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/search_index_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11787 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/search_index_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/search_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/seasonal_arima_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11615 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/segment_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11067 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/segments_list_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11948 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11760 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11610 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/unique_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/update_connection_changes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11816 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/update_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    13667 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model/why_logs_metric.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 22:40:04.477995 whylabs-client-0.5.3/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)    11040 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2023-07-13 22:39:56.000000 whylabs-client-0.5.3/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 22:40:04.452996 whylabs-client-0.5.3/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-07-13 22:40:04.000000 whylabs-client-0.5.3/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-07-13 22:40:04.000000 whylabs-client-0.5.3/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 22:40:04.000000 whylabs-client-0.5.3/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-13 22:40:04.000000 whylabs-client-0.5.3/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 22:40:04.000000 whylabs-client-0.5.3/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.5.2/PKG-INFO` & `whylabs-client-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.5.2
+Version: 0.5.3
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.5.2/README.md` & `whylabs-client-0.5.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.5.2
+- Package version: 0.5.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -120,14 +120,15 @@
 *DatasetProfileApi* | [**get_reference_profile**](docs/DatasetProfileApi.md#get_reference_profile) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Returns a single reference profile
 *DatasetProfileApi* | [**list_reference_profiles**](docs/DatasetProfileApi.md#list_reference_profiles) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles | Returns a list for reference profiles
 *DatasetMetadataApi* | [**delete_dataset_metadata**](docs/DatasetMetadataApi.md#delete_dataset_metadata) | **DELETE** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Delete dataset metadata for the specified dataset
 *DatasetMetadataApi* | [**get_dataset_metadata**](docs/DatasetMetadataApi.md#get_dataset_metadata) | **GET** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Get dataset metadata for the specified dataset
 *DatasetMetadataApi* | [**put_dataset_metadata**](docs/DatasetMetadataApi.md#put_dataset_metadata) | **PUT** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Put dataset metadata for the specified dataset
 *FeatureWeightsApi* | [**get_column_weights**](docs/FeatureWeightsApi.md#get_column_weights) | **GET** /v0/organizations/{org_id}/dataset/{dataset_id}/weights | Get column weights for the specified dataset
 *FeatureWeightsApi* | [**put_column_weights**](docs/FeatureWeightsApi.md#put_column_weights) | **PUT** /v0/organizations/{org_id}/dataset/{dataset_id}/weights | Put column weights for the specified dataset
+*LogApi* | [**get_profile_observatory_link**](docs/LogApi.md#get_profile_observatory_link) | **POST** /v0/organizations/{org_id}/log/observatory-link/{dataset_id} | Get observatory links for profiles in a given org/model. A max of 3 profiles can be viewed a a time.
 *LogApi* | [**log_async**](docs/LogApi.md#log_async) | **POST** /v0/organizations/{org_id}/log/async/{dataset_id} | Like /log, except this api doesn&#39;t take the actual profile content. It returns an upload link that can be used to upload the profile to.
 *LogApi* | [**log_reference**](docs/LogApi.md#log_reference) | **POST** /v0/organizations/{org_id}/log/reference/{model_id} | Returns a presigned URL for uploading the reference profile to.
 *MembershipApi* | [**create_organization_membership**](docs/MembershipApi.md#create_organization_membership) | **POST** /v0/organizations/{org_id}/membership | Create a membership for a user, making them apart of an organization. Uses the user&#39;s current email address.
 *MembershipApi* | [**list_organization_memberships**](docs/MembershipApi.md#list_organization_memberships) | **GET** /v0/organizations/{org_id}/membership | List organization memberships
 *MembershipApi* | [**remove_organization_membership**](docs/MembershipApi.md#remove_organization_membership) | **DELETE** /v0/organizations/{org_id}/membership | Removes membership in a given org from a user, using the user&#39;s email address.
 *MembershipApi* | [**update_organization_membership**](docs/MembershipApi.md#update_organization_membership) | **PUT** /v0/organizations/{org_id}/membership | Updates the role in an membership
 *ModelsApi* | [**create_model**](docs/ModelsApi.md#create_model) | **POST** /v0/organizations/{org_id}/models | Create a model with a given name and a time period
@@ -168,25 +169,29 @@
 *SchemaApi* | [**get_monitor_config_schema**](docs/SchemaApi.md#get_monitor_config_schema) | **GET** /v0/organizations/{org_id}/schema/monitor-config | Get the current supported schema of the monitor configuration
 *SessionsApi* | [**batch_create_reference_profile_upload**](docs/SessionsApi.md#batch_create_reference_profile_upload) | **POST** /v0/sessions/{session_id}/references | Create multiple reference profile uploads for a given session.
 *SessionsApi* | [**claim_guest_session**](docs/SessionsApi.md#claim_guest_session) | **POST** /v0/sessions/{session_id}/claim | Claim a guest session, copying its model data into another org and expiring the session.
 *SessionsApi* | [**create_dataset_profile_upload**](docs/SessionsApi.md#create_dataset_profile_upload) | **POST** /v0/sessions/{session_id}/upload | Create an upload for a given session.
 *SessionsApi* | [**create_reference_profile_upload**](docs/SessionsApi.md#create_reference_profile_upload) | **POST** /v0/sessions/{session_id}/reference | Create a reference profile upload for a given session.
 *SessionsApi* | [**create_session**](docs/SessionsApi.md#create_session) | **POST** /v0/sessions | Create a new session that can be used to upload dataset profiles from whylogs for display in whylabs.
 *SessionsApi* | [**get_session**](docs/SessionsApi.md#get_session) | **GET** /v0/sessions/{session_id} | Get information about a session.
+*SessionsApi* | [**get_session_profile_observatory_link**](docs/SessionsApi.md#get_session_profile_observatory_link) | **POST** /v0/sessions/observatory-link/{session_id} | Get observatory links for profiles in a given session. A max of 3 profiles can be viewed a a time.
 
 
 ## Documentation For Models
 
  - [AWSMarketplaceMetadata](docs/AWSMarketplaceMetadata.md)
  - [ActionType](docs/ActionType.md)
  - [AddMembershipRequest](docs/AddMembershipRequest.md)
+ - [AdminReportResponse](docs/AdminReportResponse.md)
+ - [AdminReportType](docs/AdminReportType.md)
  - [AsyncLogResponse](docs/AsyncLogResponse.md)
  - [BatchLogReferenceRequest](docs/BatchLogReferenceRequest.md)
  - [BatchLogSessionReferenceResponse](docs/BatchLogSessionReferenceResponse.md)
  - [ColumnSchema](docs/ColumnSchema.md)
+ - [CreateDatasetProfileUploadResponse](docs/CreateDatasetProfileUploadResponse.md)
  - [CreateReferenceProfileRequest](docs/CreateReferenceProfileRequest.md)
  - [CreateReferenceProfileResponse](docs/CreateReferenceProfileResponse.md)
  - [CreateSessionRequest](docs/CreateSessionRequest.md)
  - [CreateSessionResponse](docs/CreateSessionResponse.md)
  - [CreateUserRequest](docs/CreateUserRequest.md)
  - [DTOClustersAutoScaleDTO](docs/DTOClustersAutoScaleDTO.md)
  - [DTOClustersAwsAttributesDTO](docs/DTOClustersAwsAttributesDTO.md)
@@ -221,14 +226,16 @@
  - [GetConnectionResponse](docs/GetConnectionResponse.md)
  - [GetDatasetMetadataResponse](docs/GetDatasetMetadataResponse.md)
  - [GetDefaultMembershipResponse](docs/GetDefaultMembershipResponse.md)
  - [GetMarketplaceMetadataResponse](docs/GetMarketplaceMetadataResponse.md)
  - [GetMembershipsResponse](docs/GetMembershipsResponse.md)
  - [GetMonitorConfigV2Response](docs/GetMonitorConfigV2Response.md)
  - [GetNotificationSettingsResponse](docs/GetNotificationSettingsResponse.md)
+ - [GetProfileObservatoryLinkRequest](docs/GetProfileObservatoryLinkRequest.md)
+ - [GetProfileObservatoryLinkResponse](docs/GetProfileObservatoryLinkResponse.md)
  - [GetSessionResponse](docs/GetSessionResponse.md)
  - [ListJobsRequest](docs/ListJobsRequest.md)
  - [ListJobsResponse](docs/ListJobsResponse.md)
  - [ListModelsResponse](docs/ListModelsResponse.md)
  - [ListOrganizationMembershipsResponse](docs/ListOrganizationMembershipsResponse.md)
  - [ListUserApiKeys](docs/ListUserApiKeys.md)
  - [LogAsyncRequest](docs/LogAsyncRequest.md)
@@ -283,14 +290,15 @@
  - [SearchIndexType](docs/SearchIndexType.md)
  - [SearchResponse](docs/SearchResponse.md)
  - [SeasonalARIMARequestConfig](docs/SeasonalARIMARequestConfig.md)
  - [Segment](docs/Segment.md)
  - [SegmentListResponse](docs/SegmentListResponse.md)
  - [SegmentTag](docs/SegmentTag.md)
  - [SegmentWeight](docs/SegmentWeight.md)
+ - [SegmentsListRequest](docs/SegmentsListRequest.md)
  - [SessionMetadata](docs/SessionMetadata.md)
  - [SetDefaultMembershipRequest](docs/SetDefaultMembershipRequest.md)
  - [SlackNotificationAction](docs/SlackNotificationAction.md)
  - [SubscriptionTier](docs/SubscriptionTier.md)
  - [TimePeriod](docs/TimePeriod.md)
  - [UberNotificationSchedule](docs/UberNotificationSchedule.md)
  - [UniqueValuesMonitorRequestConfig](docs/UniqueValuesMonitorRequestConfig.md)
```

### Comparing `whylabs-client-0.5.2/setup.py` & `whylabs-client-0.5.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "RELEASE.md").read_text()
 
 NAME = "whylabs-client"
-VERSION = "0.5.2"
+VERSION = "0.5.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `whylabs-client-0.5.2/whylabs_client/__init__.py` & `whylabs-client-0.5.3/whylabs_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.5.2/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.5.3/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.5.3/whylabs_client/api/dataset_profile_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.5.3/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/membership_api.py` & `whylabs-client-0.5.3/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/models_api.py` & `whylabs-client-0.5.3/whylabs_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/monitor_api.py` & `whylabs-client-0.5.3/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.5.3/whylabs_client/api/notification_settings_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/schema_api.py` & `whylabs-client-0.5.3/whylabs_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/api/sessions_api.py` & `whylabs-client-0.5.3/whylabs_client/api/sessions_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,19 +18,21 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from whylabs_client.model.async_log_response import AsyncLogResponse
 from whylabs_client.model.batch_log_reference_request import BatchLogReferenceRequest
 from whylabs_client.model.batch_log_session_reference_response import BatchLogSessionReferenceResponse
+from whylabs_client.model.create_dataset_profile_upload_response import CreateDatasetProfileUploadResponse
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
+from whylabs_client.model.get_profile_observatory_link_request import GetProfileObservatoryLinkRequest
+from whylabs_client.model.get_profile_observatory_link_response import GetProfileObservatoryLinkResponse
 from whylabs_client.model.get_session_response import GetSessionResponse
 from whylabs_client.model.log_async_request import LogAsyncRequest
 from whylabs_client.model.log_reference_request import LogReferenceRequest
 from whylabs_client.model.log_session_reference_response import LogSessionReferenceResponse
 
 
 class SessionsApi(object):
@@ -155,15 +157,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.create_dataset_profile_upload_endpoint = _Endpoint(
             settings={
-                'response_type': (AsyncLogResponse,),
+                'response_type': (CreateDatasetProfileUploadResponse,),
                 'auth': [],
                 'endpoint_path': '/v0/sessions/{session_id}/upload',
                 'operation_id': 'create_dataset_profile_upload',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
@@ -366,14 +368,70 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_session_profile_observatory_link_endpoint = _Endpoint(
+            settings={
+                'response_type': (GetProfileObservatoryLinkResponse,),
+                'auth': [],
+                'endpoint_path': '/v0/sessions/observatory-link/{session_id}',
+                'operation_id': 'get_session_profile_observatory_link',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'session_id',
+                    'get_profile_observatory_link_request',
+                ],
+                'required': [
+                    'session_id',
+                    'get_profile_observatory_link_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'session_id':
+                        (str,),
+                    'get_profile_observatory_link_request':
+                        (GetProfileObservatoryLinkRequest,),
+                },
+                'attribute_map': {
+                    'session_id': 'session_id',
+                },
+                'location_map': {
+                    'session_id': 'path',
+                    'get_profile_observatory_link_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
 
     def batch_create_reference_profile_upload(
         self,
         session_id,
         batch_log_reference_request,
         **kwargs
     ):
@@ -561,15 +619,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            AsyncLogResponse
+            CreateDatasetProfileUploadResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -809,7 +867,82 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['session_id'] = \
             session_id
         return self.get_session_endpoint.call_with_http_info(**kwargs)
 
+    def get_session_profile_observatory_link(
+        self,
+        session_id,
+        get_profile_observatory_link_request,
+        **kwargs
+    ):
+        """Get observatory links for profiles in a given session. A max of 3 profiles can be viewed a a time.  # noqa: E501
+
+        Get observatory links for profiles in a given session. A max of 3 profiles can be viewed a a time.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_session_profile_observatory_link(session_id, get_profile_observatory_link_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            session_id (str):
+            get_profile_observatory_link_request (GetProfileObservatoryLinkRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            GetProfileObservatoryLinkResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['session_id'] = \
+            session_id
+        kwargs['get_profile_observatory_link_request'] = \
+            get_profile_observatory_link_request
+        return self.get_session_profile_observatory_link_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `whylabs-client-0.5.2/whylabs_client/api_client.py` & `whylabs-client-0.5.3/whylabs_client/api_client.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/apis/__init__.py` & `whylabs-client-0.5.3/whylabs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/configuration.py` & `whylabs-client-0.5.3/whylabs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.5.2".\
+               "SDK Package Version: 0.5.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.5.2/whylabs_client/exceptions.py` & `whylabs-client-0.5.3/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/action_type.py` & `whylabs-client-0.5.3/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.5.3/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/async_log_response.py` & `whylabs-client-0.5.3/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.5.3/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/batch_log_reference_request.py` & `whylabs-client-0.5.3/whylabs_client/model/batch_log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/batch_log_session_reference_response.py` & `whylabs-client-0.5.3/whylabs_client/model/batch_log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/column_schema.py` & `whylabs-client-0.5.3/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/create_reference_profile_request.py` & `whylabs-client-0.5.3/whylabs_client/model/create_reference_profile_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/create_reference_profile_response.py` & `whylabs-client-0.5.3/whylabs_client/model/create_reference_profile_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/create_session_request.py` & `whylabs-client-0.5.3/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/create_session_response.py` & `whylabs-client-0.5.3/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/create_user_request.py` & `whylabs-client-0.5.3/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/databricks_connection.py` & `whylabs-client-0.5.3/whylabs_client/model/databricks_connection.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dataset_request_monitor_config.py` & `whylabs-client-0.5.3/whylabs_client/model/dataset_request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/datatype_monitor_request_config.py` & `whylabs-client-0.5.3/whylabs_client/model/datatype_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.5.3/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.5.3/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/distribution_monitor_request_config.py` & `whylabs-client-0.5.3/whylabs_client/model/distribution_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_clusters_auto_scale_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_clusters_auto_scale_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_clusters_aws_attributes_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_clusters_aws_attributes_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_clusters_aws_availability_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_clusters_aws_availability_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_clusters_s3_storage_info_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_clusters_s3_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_ebs_volume_type_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_ebs_volume_type_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_cron_schedule_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_cron_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_data_security_mode_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_data_security_mode_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_job_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_job_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_job_email_notifications_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_job_email_notifications_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_job_settings_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_job_settings_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_new_cluster_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_new_cluster_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_notebook_task_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_notebook_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_spark_jar_task_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_spark_jar_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_spark_python_task_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_spark_python_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/dto_jobs_spark_submit_task_dto.py` & `whylabs-client-0.5.3/whylabs_client/model/dto_jobs_spark_submit_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.5.3/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/entity_schema.py` & `whylabs-client-0.5.3/whylabs_client/model/entity_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/entity_search_result.py` & `whylabs-client-0.5.3/whylabs_client/model/entity_search_result.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.5.3/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.5.3/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/feature_flags.py` & `whylabs-client-0.5.3/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_connection_request.py` & `whylabs-client-0.5.3/whylabs_client/model/get_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_connection_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_monitor_config_v2_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_monitor_config_v2_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/get_session_response.py` & `whylabs-client-0.5.3/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/list_jobs_request.py` & `whylabs-client-0.5.3/whylabs_client/model/list_jobs_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/list_jobs_response.py` & `whylabs-client-0.5.3/whylabs_client/model/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/list_models_response.py` & `whylabs-client-0.5.3/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.5.3/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.5.3/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/log_async_request.py` & `whylabs-client-0.5.3/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.5.3/whylabs_client/model/log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.5.3/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/log_response.py` & `whylabs-client-0.5.3/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/log_session_reference_response.py` & `whylabs-client-0.5.3/whylabs_client/model/log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.5.3/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/membership.py` & `whylabs-client-0.5.3/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.5.3/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/metric_schema.py` & `whylabs-client-0.5.3/whylabs_client/model/metric_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/missing_recent_data_request_config.py` & `whylabs-client-0.5.3/whylabs_client/model/missing_recent_data_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/missing_recent_profiles_request_config.py` & `whylabs-client-0.5.3/whylabs_client/model/missing_recent_profiles_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/missing_values_monitor_request_config.py` & `whylabs-client-0.5.3/whylabs_client/model/missing_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.5.3/whylabs_client/model/model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/model_type.py` & `whylabs-client-0.5.3/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/monitor_config.py` & `whylabs-client-0.5.3/whylabs_client/model/monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.5.3/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/monitor_request_reference.py` & `whylabs-client-0.5.3/whylabs_client/model/monitor_request_reference.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/monitor_request_reference_type.py` & `whylabs-client-0.5.3/whylabs_client/model/monitor_request_reference_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/notification_action.py` & `whylabs-client-0.5.3/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/notification_relationship_item.py` & `whylabs-client-0.5.3/whylabs_client/model/notification_relationship_item.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/notification_relationship_type.py` & `whylabs-client-0.5.3/whylabs_client/model/notification_relationship_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/notification_settings.py` & `whylabs-client-0.5.3/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.5.3/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.5.3/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.5.3/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/organization_summary.py` & `whylabs-client-0.5.3/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.5.3/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/provided_config.py` & `whylabs-client-0.5.3/whylabs_client/model/provided_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/provision_databricks_connection_request.py` & `whylabs-client-0.5.3/whylabs_client/model/provision_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/provision_databricks_connection_response.py` & `whylabs-client-0.5.3/whylabs_client/model/provision_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.5.3/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.5.3/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.5.3/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.5.3/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.5.3/whylabs_client/model/reference_profile_item_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/refresh_access_token_request.py` & `whylabs-client-0.5.3/whylabs_client/model/refresh_access_token_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/refresh_connection_by_org_id_response.py` & `whylabs-client-0.5.3/whylabs_client/model/refresh_connection_by_org_id_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/refresh_connection_request.py` & `whylabs-client-0.5.3/whylabs_client/model/refresh_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/register_databricks_connection_request.py` & `whylabs-client-0.5.3/whylabs_client/model/register_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/register_databricks_connection_response.py` & `whylabs-client-0.5.3/whylabs_client/model/register_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.5.3/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/request_feature_monitor_config.py` & `whylabs-client-0.5.3/whylabs_client/model/request_feature_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/request_monitor_config.py` & `whylabs-client-0.5.3/whylabs_client/model/request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/response.py` & `whylabs-client-0.5.3/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/role.py` & `whylabs-client-0.5.3/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/run_job_request.py` & `whylabs-client-0.5.3/whylabs_client/model/run_job_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/run_job_response.py` & `whylabs-client-0.5.3/whylabs_client/model/run_job_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.5.3/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/search_index_request.py` & `whylabs-client-0.5.3/whylabs_client/model/search_index_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/search_index_type.py` & `whylabs-client-0.5.3/whylabs_client/model/search_index_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/search_response.py` & `whylabs-client-0.5.3/whylabs_client/model/search_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/seasonal_arima_request_config.py` & `whylabs-client-0.5.3/whylabs_client/model/seasonal_arima_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/segment.py` & `whylabs-client-0.5.3/whylabs_client/model/segment.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/segment_list_response.py` & `whylabs-client-0.5.3/whylabs_client/model/segment_list_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/segment_tag.py` & `whylabs-client-0.5.3/whylabs_client/model/segment_tag.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/segment_weight.py` & `whylabs-client-0.5.3/whylabs_client/model/segment_weight.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/session_metadata.py` & `whylabs-client-0.5.3/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.5.3/whylabs_client/model/set_default_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.5.3/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.5.3/whylabs_client/model/subscription_tier.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/time_period.py` & `whylabs-client-0.5.3/whylabs_client/model/time_period.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.5.3/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/unique_values_monitor_request_config.py` & `whylabs-client-0.5.3/whylabs_client/model/unique_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/update_connection_changes.py` & `whylabs-client-0.5.3/whylabs_client/model/update_connection_changes.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/update_connection_request.py` & `whylabs-client-0.5.3/whylabs_client/model/update_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.5.3/whylabs_client/model/update_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/user.py` & `whylabs-client-0.5.3/whylabs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/user_api_key.py` & `whylabs-client-0.5.3/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.5.3/whylabs_client/model/user_api_key_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model/why_logs_metric.py` & `whylabs-client-0.5.3/whylabs_client/model/why_logs_metric.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/model_utils.py` & `whylabs-client-0.5.3/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client/models/__init__.py` & `whylabs-client-0.5.3/whylabs_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from whylabs_client.model.aws_marketplace_metadata import AWSMarketplaceMetadata
 from whylabs_client.model.action_type import ActionType
 from whylabs_client.model.add_membership_request import AddMembershipRequest
+from whylabs_client.model.admin_report_response import AdminReportResponse
+from whylabs_client.model.admin_report_type import AdminReportType
 from whylabs_client.model.async_log_response import AsyncLogResponse
 from whylabs_client.model.batch_log_reference_request import BatchLogReferenceRequest
 from whylabs_client.model.batch_log_session_reference_response import BatchLogSessionReferenceResponse
 from whylabs_client.model.column_schema import ColumnSchema
+from whylabs_client.model.create_dataset_profile_upload_response import CreateDatasetProfileUploadResponse
 from whylabs_client.model.create_reference_profile_request import CreateReferenceProfileRequest
 from whylabs_client.model.create_reference_profile_response import CreateReferenceProfileResponse
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
 from whylabs_client.model.create_user_request import CreateUserRequest
 from whylabs_client.model.dto_clusters_auto_scale_dto import DTOClustersAutoScaleDTO
 from whylabs_client.model.dto_clusters_aws_attributes_dto import DTOClustersAwsAttributesDTO
@@ -54,14 +57,16 @@
 from whylabs_client.model.get_connection_response import GetConnectionResponse
 from whylabs_client.model.get_dataset_metadata_response import GetDatasetMetadataResponse
 from whylabs_client.model.get_default_membership_response import GetDefaultMembershipResponse
 from whylabs_client.model.get_marketplace_metadata_response import GetMarketplaceMetadataResponse
 from whylabs_client.model.get_memberships_response import GetMembershipsResponse
 from whylabs_client.model.get_monitor_config_v2_response import GetMonitorConfigV2Response
 from whylabs_client.model.get_notification_settings_response import GetNotificationSettingsResponse
+from whylabs_client.model.get_profile_observatory_link_request import GetProfileObservatoryLinkRequest
+from whylabs_client.model.get_profile_observatory_link_response import GetProfileObservatoryLinkResponse
 from whylabs_client.model.get_session_response import GetSessionResponse
 from whylabs_client.model.list_jobs_request import ListJobsRequest
 from whylabs_client.model.list_jobs_response import ListJobsResponse
 from whylabs_client.model.list_models_response import ListModelsResponse
 from whylabs_client.model.list_organization_memberships_response import ListOrganizationMembershipsResponse
 from whylabs_client.model.list_user_api_keys import ListUserApiKeys
 from whylabs_client.model.log_async_request import LogAsyncRequest
@@ -116,14 +121,15 @@
 from whylabs_client.model.search_index_type import SearchIndexType
 from whylabs_client.model.search_response import SearchResponse
 from whylabs_client.model.seasonal_arima_request_config import SeasonalARIMARequestConfig
 from whylabs_client.model.segment import Segment
 from whylabs_client.model.segment_list_response import SegmentListResponse
 from whylabs_client.model.segment_tag import SegmentTag
 from whylabs_client.model.segment_weight import SegmentWeight
+from whylabs_client.model.segments_list_request import SegmentsListRequest
 from whylabs_client.model.session_metadata import SessionMetadata
 from whylabs_client.model.set_default_membership_request import SetDefaultMembershipRequest
 from whylabs_client.model.slack_notification_action import SlackNotificationAction
 from whylabs_client.model.subscription_tier import SubscriptionTier
 from whylabs_client.model.time_period import TimePeriod
 from whylabs_client.model.uber_notification_schedule import UberNotificationSchedule
 from whylabs_client.model.unique_values_monitor_request_config import UniqueValuesMonitorRequestConfig
```

### Comparing `whylabs-client-0.5.2/whylabs_client/rest.py` & `whylabs-client-0.5.3/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.2/whylabs_client.egg-info/PKG-INFO` & `whylabs-client-0.5.3/whylabs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.5.2
+Version: 0.5.3
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.5.2/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.5.3/whylabs_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,22 @@
 whylabs_client/api/notification_settings_api.py
 whylabs_client/api/schema_api.py
 whylabs_client/api/sessions_api.py
 whylabs_client/apis/__init__.py
 whylabs_client/model/__init__.py
 whylabs_client/model/action_type.py
 whylabs_client/model/add_membership_request.py
+whylabs_client/model/admin_report_response.py
+whylabs_client/model/admin_report_type.py
 whylabs_client/model/async_log_response.py
 whylabs_client/model/aws_marketplace_metadata.py
 whylabs_client/model/batch_log_reference_request.py
 whylabs_client/model/batch_log_session_reference_response.py
 whylabs_client/model/column_schema.py
+whylabs_client/model/create_dataset_profile_upload_response.py
 whylabs_client/model/create_reference_profile_request.py
 whylabs_client/model/create_reference_profile_response.py
 whylabs_client/model/create_session_request.py
 whylabs_client/model/create_session_response.py
 whylabs_client/model/create_user_request.py
 whylabs_client/model/databricks_connection.py
 whylabs_client/model/dataset_request_monitor_config.py
@@ -70,14 +73,16 @@
 whylabs_client/model/get_connection_response.py
 whylabs_client/model/get_dataset_metadata_response.py
 whylabs_client/model/get_default_membership_response.py
 whylabs_client/model/get_marketplace_metadata_response.py
 whylabs_client/model/get_memberships_response.py
 whylabs_client/model/get_monitor_config_v2_response.py
 whylabs_client/model/get_notification_settings_response.py
+whylabs_client/model/get_profile_observatory_link_request.py
+whylabs_client/model/get_profile_observatory_link_response.py
 whylabs_client/model/get_session_response.py
 whylabs_client/model/list_jobs_request.py
 whylabs_client/model/list_jobs_response.py
 whylabs_client/model/list_models_response.py
 whylabs_client/model/list_organization_memberships_response.py
 whylabs_client/model/list_user_api_keys.py
 whylabs_client/model/log_async_request.py
@@ -132,14 +137,15 @@
 whylabs_client/model/search_index_type.py
 whylabs_client/model/search_response.py
 whylabs_client/model/seasonal_arima_request_config.py
 whylabs_client/model/segment.py
 whylabs_client/model/segment_list_response.py
 whylabs_client/model/segment_tag.py
 whylabs_client/model/segment_weight.py
+whylabs_client/model/segments_list_request.py
 whylabs_client/model/session_metadata.py
 whylabs_client/model/set_default_membership_request.py
 whylabs_client/model/slack_notification_action.py
 whylabs_client/model/subscription_tier.py
 whylabs_client/model/time_period.py
 whylabs_client/model/uber_notification_schedule.py
 whylabs_client/model/unique_values_monitor_request_config.py
```

