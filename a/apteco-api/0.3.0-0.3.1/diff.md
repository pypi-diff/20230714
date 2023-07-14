# Comparing `tmp/apteco-api-0.3.0.tar.gz` & `tmp/apteco-api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\apteco-api-0.3.0.tar", last modified: Fri Jun 30 12:33:01 2023, max compression
+gzip compressed data, was "dist\apteco-api-0.3.1.tar", last modified: Fri Jul 14 11:46:03 2023, max compression
```

## Comparing `apteco-api-0.3.0.tar` & `apteco-api-0.3.1.tar`

### file list

```diff
@@ -1,363 +1,363 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 12:33:01.510775 apteco-api-0.3.0/
--rw-rw-rw-   0        0        0    11556 2019-06-24 15:29:29.000000 apteco-api-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     9760 2023-06-30 12:33:01.510197 apteco-api-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 12:33:00.900440 apteco-api-0.3.0/pkg/
-drwxrwxrwx   0        0        0        0 2023-06-30 12:33:00.908440 apteco-api-0.3.0/pkg/apteco_api/
--rw-rw-rw-   0        0        0    25109 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:33:00.954154 apteco-api-0.3.0/pkg/apteco_api/api/
--rw-rw-rw-   0        0        0     2033 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/__init__.py
--rw-rw-rw-   0        0        0    85079 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/about_api.py
--rw-rw-rw-   0        0        0    48087 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/audience_compositions_api.py
--rw-rw-rw-   0        0        0    15326 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/audience_hits_api.py
--rw-rw-rw-   0        0        0    15768 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/audience_settings_api.py
--rw-rw-rw-   0        0        0   231588 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/audiences_api.py
--rw-rw-rw-   0        0        0    15454 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/collection_hits_api.py
--rw-rw-rw-   0        0        0    80868 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/collections_api.py
--rw-rw-rw-   0        0        0     8864 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/cubes_api.py
--rw-rw-rw-   0        0        0   106812 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/dashboards_api.py
--rw-rw-rw-   0        0        0    72595 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/data_licensing_api.py
--rw-rw-rw-   0        0        0    45146 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/directories_api.py
--rw-rw-rw-   0        0        0    23649 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/exports_api.py
--rw-rw-rw-   0        0        0    13970 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/external_login_api.py
--rw-rw-rw-   0        0        0    29841 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/fast_stats_builds_api.py
--rw-rw-rw-   0        0        0    47064 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/fast_stats_jobs_api.py
--rw-rw-rw-   0        0        0   102470 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/fast_stats_systems_api.py
--rw-rw-rw-   0        0        0    33501 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/files_api.py
--rw-rw-rw-   0        0        0    32961 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/groups_api.py
--rw-rw-rw-   0        0        0   116442 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/api/people_stage_api.py
--rw-rw-rw-   0        0        0   107622 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/permissions_api.py
--rw-rw-rw-   0        0        0    31868 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/queries_api.py
--rw-rw-rw-   0        0        0    55519 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/sessions_api.py
--rw-rw-rw-   0        0        0    37597 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/settings_api.py
--rw-rw-rw-   0        0        0    85237 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/shares_api.py
--rw-rw-rw-   0        0        0    54038 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/static_resources_api.py
--rw-rw-rw-   0        0        0    33581 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/teams_api.py
--rw-rw-rw-   0        0        0    48032 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/telemetry_api.py
--rw-rw-rw-   0        0        0    29192 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/temporary_files_api.py
--rw-rw-rw-   0        0        0    36096 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/themes_api.py
--rw-rw-rw-   0        0        0    28429 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/user_registration_requests_api.py
--rw-rw-rw-   0        0        0    28956 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/user_reset_password_requests_api.py
--rw-rw-rw-   0        0        0   145025 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/users_api.py
--rw-rw-rw-   0        0        0    41797 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api/visualisations_api.py
--rw-rw-rw-   0        0        0    26203 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/api_client.py
--rw-rw-rw-   0        0        0    13310 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/configuration.py
--rw-rw-rw-   0        0        0     3768 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:33:01.509197 apteco-api-0.3.0/pkg/apteco_api/models/
--rw-rw-rw-   0        0        0    22755 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/models/__init__.py
--rw-rw-rw-   0        0        0    13413 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/abstract_render_spec.py
--rw-rw-rw-   0        0        0     8275 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/age_rule.py
--rw-rw-rw-   0        0        0     7533 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_calculate_job_detail.py
--rw-rw-rw-   0        0        0     9455 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_check_detail.py
--rw-rw-rw-   0        0        0     7414 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_check_job_detail.py
--rw-rw-rw-   0        0        0     7684 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_data_licensing_info_job_detail.py
--rw-rw-rw-   0        0        0    24859 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_detail.py
--rw-rw-rw-   0        0        0    15757 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_export_detail.py
--rw-rw-rw-   0        0        0     7461 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_export_job_detail.py
--rw-rw-rw-   0        0        0     7304 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_hit_detail.py
--rw-rw-rw-   0        0        0     6299 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_hit_summary.py
--rw-rw-rw-   0        0        0     4344 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_query_result.py
--rw-rw-rw-   0        0        0    12937 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_result_detail.py
--rw-rw-rw-   0        0        0    10239 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_result_summary.py
--rw-rw-rw-   0        0        0     7233 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_settings_detail.py
--rw-rw-rw-   0        0        0     7249 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_settings_summary.py
--rw-rw-rw-   0        0        0    19344 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_summary.py
--rw-rw-rw-   0        0        0    14648 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_update_detail.py
--rw-rw-rw-   0        0        0    10513 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/audience_update_summary.py
--rw-rw-rw-   0        0        0    12463 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/authorised_permission.py
--rw-rw-rw-   0        0        0     4673 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/authorised_permission_with_lookups.py
--rw-rw-rw-   0        0        0     3892 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/authority.py
--rw-rw-rw-   0        0        0     7220 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/breakpoint.py
--rw-rw-rw-   0        0        0     3612 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/build_definition.py
--rw-rw-rw-   0        0        0     7158 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/build_job_detail.py
--rw-rw-rw-   0        0        0     3571 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/build_result.py
--rw-rw-rw-   0        0        0     3911 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/calculate_audience_details.py
--rw-rw-rw-   0        0        0     4828 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/calculate_dashboard_data.py
--rw-rw-rw-   0        0        0     6419 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/calculate_dashboard_item.py
--rw-rw-rw-   0        0        0     5340 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/calculate_dashboard_item_job_created_result.py
--rw-rw-rw-   0        0        0     6532 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/capabilities.py
--rw-rw-rw-   0        0        0     4838 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/change_password_details.py
--rw-rw-rw-   0        0        0     7450 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/channel_detail.py
--rw-rw-rw-   0        0        0     8317 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/channel_statistics.py
--rw-rw-rw-   0        0        0     7474 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/channel_summary.py
--rw-rw-rw-   0        0        0     3845 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/check_audience_details.py
--rw-rw-rw-   0        0        0     5022 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/check_composition_definition.py
--rw-rw-rw-   0        0        0     7934 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/check_dimension_result.py
--rw-rw-rw-   0        0        0     4620 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/clause.py
--rw-rw-rw-   0        0        0    15886 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/collection_detail.py
--rw-rw-rw-   0        0        0     7398 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/collection_hit_detail.py
--rw-rw-rw-   0        0        0     6385 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/collection_hit_summary.py
--rw-rw-rw-   0        0        0     8098 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/collection_part_detail.py
--rw-rw-rw-   0        0        0     7234 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/collection_part_summary.py
--rw-rw-rw-   0        0        0    15078 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/collection_summary.py
--rw-rw-rw-   0        0        0    10066 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/column.py
--rw-rw-rw-   0        0        0    20298 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/communication_statistics.py
--rw-rw-rw-   0        0        0    14227 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/composition_detail.py
--rw-rw-rw-   0        0        0    11029 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/composition_summary.py
--rw-rw-rw-   0        0        0     4903 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/confirm_reset_password_request.py
--rw-rw-rw-   0        0        0     4344 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/convert_dashboard_to_audience.py
--rw-rw-rw-   0        0        0     3534 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/convert_dashboard_to_audience_result.py
--rw-rw-rw-   0        0        0     3661 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/copy_audience_detail.py
--rw-rw-rw-   0        0        0     3671 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/copy_dashboard_detail.py
--rw-rw-rw-   0        0        0     4607 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/count.py
--rw-rw-rw-   0        0        0     7500 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_audience_composition_detail.py
--rw-rw-rw-   0        0        0     9647 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_audience_detail.py
--rw-rw-rw-   0        0        0     3759 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_audience_hit_details.py
--rw-rw-rw-   0        0        0     9258 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_audience_update.py
--rw-rw-rw-   0        0        0     3775 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_collection_hit_details.py
--rw-rw-rw-   0        0        0     8600 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_dashboard_detail.py
--rw-rw-rw-   0        0        0     9663 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_dashboard_update_detail.py
--rw-rw-rw-   0        0        0     6102 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_reset_password_request.py
--rw-rw-rw-   0        0        0     8879 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_session_parameters.py
--rw-rw-rw-   0        0        0    15507 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_share_detail.py
--rw-rw-rw-   0        0        0    20708 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_share_update.py
--rw-rw-rw-   0        0        0     3525 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_team_details.py
--rw-rw-rw-   0        0        0     6201 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_telemetry_session_details.py
--rw-rw-rw-   0        0        0     3713 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_telemetry_state_details.py
--rw-rw-rw-   0        0        0     7229 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_update_theme.py
--rw-rw-rw-   0        0        0     7918 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_user_details.py
--rw-rw-rw-   0        0        0     9268 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/create_user_registration_request.py
--rw-rw-rw-   0        0        0     6843 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/created_share_update_detail.py
--rw-rw-rw-   0        0        0    10949 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/criteria.py
--rw-rw-rw-   0        0        0     8225 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/cube.py
--rw-rw-rw-   0        0        0    13307 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/cube_result.py
--rw-rw-rw-   0        0        0     4394 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/cube_specification.py
--rw-rw-rw-   0        0        0     6461 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_content_item.py
--rw-rw-rw-   0        0        0    14979 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_content_item_detail.py
--rw-rw-rw-   0        0        0    19161 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_detail.py
--rw-rw-rw-   0        0        0     3635 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_export_data.py
--rw-rw-rw-   0        0        0     4591 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_export_data_result.py
--rw-rw-rw-   0        0        0     9714 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item.py
--rw-rw-rw-   0        0        0     7181 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_category_display.py
--rw-rw-rw-   0        0        0     6405 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data.py
--rw-rw-rw-   0        0        0     5548 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_job_created.py
--rw-rw-rw-   0        0        0     8532 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_job_detail.py
--rw-rw-rw-   0        0        0     6117 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_result_detail.py
--rw-rw-rw-   0        0        0     4716 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_specification.py
--rw-rw-rw-   0        0        0     8507 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_preview_data.py
--rw-rw-rw-   0        0        0     3628 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/data_licensing_detail.py
--rw-rw-rw-   0        0        0     4761 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/data_licensing_system_detail.py
--rw-rw-rw-   0        0        0     4773 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/data_licensing_system_summary.py
--rw-rw-rw-   0        0        0     9206 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/data_purchase_detail.py
--rw-rw-rw-   0        0        0     7349 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/data_purchase_job_detail.py
--rw-rw-rw-   0        0        0     4445 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/data_view_details.py
--rw-rw-rw-   0        0        0     3507 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/data_view_summary.py
--rw-rw-rw-   0        0        0    26245 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/date_rule.py
--rw-rw-rw-   0        0        0     6788 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/date_settings.py
--rw-rw-rw-   0        0        0     4046 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/diagram_metadata.py
--rw-rw-rw-   0        0        0    16094 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dimension.py
--rw-rw-rw-   0        0        0     5218 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dimension_banding.py
--rw-rw-rw-   0        0        0     5808 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/dimension_result.py
--rw-rw-rw-   0        0        0    11353 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/element_detail.py
--rw-rw-rw-   0        0        0     4375 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/element_key.py
--rw-rw-rw-   0        0        0    15738 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/element_status.py
--rw-rw-rw-   0        0        0    11389 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/element_summary.py
--rw-rw-rw-   0        0        0     6116 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/email_requirements.py
--rw-rw-rw-   0        0        0    15650 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/endpoint_details.py
--rw-rw-rw-   0        0        0     5844 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/error_message.py
--rw-rw-rw-   0        0        0     3920 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/error_message_parameter.py
--rw-rw-rw-   0        0        0    10554 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/export.py
--rw-rw-rw-   0        0        0     9405 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/export_audience_details.py
--rw-rw-rw-   0        0        0     4653 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/export_composition_definition.py
--rw-rw-rw-   0        0        0    11938 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/export_result.py
--rw-rw-rw-   0        0        0     5630 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/export_system_detail.py
--rw-rw-rw-   0        0        0     5646 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/export_system_summary.py
--rw-rw-rw-   0        0        0     8685 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/expression.py
--rw-rw-rw-   0        0        0     7829 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/fast_stats_system_detail.py
--rw-rw-rw-   0        0        0     6591 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/fast_stats_system_item.py
--rw-rw-rw-   0        0        0     6867 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/fast_stats_system_summary.py
--rw-rw-rw-   0        0        0     5663 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/file_entry.py
--rw-rw-rw-   0        0        0    10746 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/file_stream.py
--rw-rw-rw-   0        0        0     3729 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/file_system_summary.py
--rw-rw-rw-   0        0        0     4389 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/folder.py
--rw-rw-rw-   0        0        0     4040 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/folder_structure_node.py
--rw-rw-rw-   0        0        0     4004 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/fraction.py
--rw-rw-rw-   0        0        0     7564 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/grid_item.py
--rw-rw-rw-   0        0        0     4218 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/group_detail.py
--rw-rw-rw-   0        0        0     4230 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/group_summary.py
--rw-rw-rw-   0        0        0     4513 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/id.py
--rw-rw-rw-   0        0        0     9065 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/invalid_to_share_user_display_details.py
--rw-rw-rw-   0        0        0    15996 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/job_detail.py
--rw-rw-rw-   0        0        0    14284 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/job_summary.py
--rw-rw-rw-   0        0        0     4187 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/language_details.py
--rw-rw-rw-   0        0        0     5591 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/last_run_details.py
--rw-rw-rw-   0        0        0    11076 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/licence.py
--rw-rw-rw-   0        0        0     7298 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/licensing_info.py
--rw-rw-rw-   0        0        0     3339 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/licensing_set.py
--rw-rw-rw-   0        0        0     7535 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/licensing_sets_job_detail.py
--rw-rw-rw-   0        0        0     7764 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/limits.py
--rw-rw-rw-   0        0        0     7392 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/link.py
--rw-rw-rw-   0        0        0     5424 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/list_rule.py
--rw-rw-rw-   0        0        0     5695 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/logic.py
--rw-rw-rw-   0        0        0     5038 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/lookups.py
--rw-rw-rw-   0        0        0    10329 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/measure.py
--rw-rw-rw-   0        0        0     6220 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/measure_result.py
--rw-rw-rw-   0        0        0     3441 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/message.py
--rw-rw-rw-   0        0        0     4647 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/model_property.py
--rw-rw-rw-   0        0        0     4970 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_items_modify_user_audience.py
--rw-rw-rw-   0        0        0     5000 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_items_modify_user_collection.py
--rw-rw-rw-   0        0        0     4985 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_items_modify_user_dashboard.py
--rw-rw-rw-   0        0        0     6108 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_audience.py
--rw-rw-rw-   0        0        0     9642 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_audience_detail.py
--rw-rw-rw-   0        0        0     7502 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_audience_detail_results.py
--rw-rw-rw-   0        0        0     6188 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_collection.py
--rw-rw-rw-   0        0        0     6393 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_collection_detail.py
--rw-rw-rw-   0        0        0     7596 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_collection_detail_results.py
--rw-rw-rw-   0        0        0     6148 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_dashboard.py
--rw-rw-rw-   0        0        0    10730 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_dashboard_detail.py
--rw-rw-rw-   0        0        0     7549 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/modify_user_dashboard_detail_results.py
--rw-rw-rw-   0        0        0     5038 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/n_per.py
--rw-rw-rw-   0        0        0     7898 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/notes_alignment.py
--rw-rw-rw-   0        0        0     7559 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/numeric_variable_info.py
--rw-rw-rw-   0        0        0     8664 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/output.py
--rw-rw-rw-   0        0        0     5608 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/output_type.py
--rw-rw-rw-   0        0        0     6876 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_hit_summary.py
--rw-rw-rw-   0        0        0     6945 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_result_summary.py
--rw-rw-rw-   0        0        0     6991 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_settings_summary.py
--rw-rw-rw-   0        0        0     6807 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_summary.py
--rw-rw-rw-   0        0        0     6945 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_update_summary.py
--rw-rw-rw-   0        0        0     7175 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_authorised_permission_with_lookups.py
--rw-rw-rw-   0        0        0     6784 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_channel_summary.py
--rw-rw-rw-   0        0        0     6922 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_collection_hit_summary.py
--rw-rw-rw-   0        0        0     6945 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_collection_part_summary.py
--rw-rw-rw-   0        0        0     6853 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_collection_summary.py
--rw-rw-rw-   0        0        0     6876 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_composition_summary.py
--rw-rw-rw-   0        0        0     7060 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_data_licensing_system_summary.py
--rw-rw-rw-   0        0        0     6807 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_data_view_summary.py
--rw-rw-rw-   0        0        0     6761 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_element_status.py
--rw-rw-rw-   0        0        0     6784 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_element_summary.py
--rw-rw-rw-   0        0        0     6807 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_endpoint_details.py
--rw-rw-rw-   0        0        0     6899 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_export_system_summary.py
--rw-rw-rw-   0        0        0     6899 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_fast_stats_system_item.py
--rw-rw-rw-   0        0        0     6968 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_fast_stats_system_summary.py
--rw-rw-rw-   0        0        0     6669 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_file_entry.py
--rw-rw-rw-   0        0        0     6853 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_file_system_summary.py
--rw-rw-rw-   0        0        0     6899 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_folder_structure_node.py
--rw-rw-rw-   0        0        0     6715 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_group_detail.py
--rw-rw-rw-   0        0        0     6738 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_group_summary.py
--rw-rw-rw-   0        0        0     6692 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_job_summary.py
--rw-rw-rw-   0        0        0     6738 2023-06-30 12:18:57.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_licensing_set.py
--rw-rw-rw-   0        0        0     7175 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_modify_user_audience_detail_results.py
--rw-rw-rw-   0        0        0     7221 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_modify_user_collection_detail_results.py
--rw-rw-rw-   0        0        0     7198 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_modify_user_dashboard_detail_results.py
--rw-rw-rw-   0        0        0     7014 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_people_stage_system_summary.py
--rw-rw-rw-   0        0        0     6991 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_resource_category_summary.py
--rw-rw-rw-   0        0        0     6807 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_resource_summary.py
--rw-rw-rw-   0        0        0     6945 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_session_and_user_details.py
--rw-rw-rw-   0        0        0     6738 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_share_summary.py
--rw-rw-rw-   0        0        0     6715 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_share_update.py
--rw-rw-rw-   0        0        0     6577 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_table.py
--rw-rw-rw-   0        0        0     6715 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_team_summary.py
--rw-rw-rw-   0        0        0     7152 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_audience_composition_summary.py
--rw-rw-rw-   0        0        0     6899 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_audience_summary.py
--rw-rw-rw-   0        0        0     6945 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_collection_summary.py
--rw-rw-rw-   0        0        0     6922 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_dashboard_summary.py
--rw-rw-rw-   0        0        0     6876 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_display_details.py
--rw-rw-rw-   0        0        0     6669 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_login.py
--rw-rw-rw-   0        0        0     7152 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_registration_request_summary.py
--rw-rw-rw-   0        0        0     6715 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_summary.py
--rw-rw-rw-   0        0        0     6623 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_var_code.py
--rw-rw-rw-   0        0        0     6646 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/paged_results_variable.py
--rw-rw-rw-   0        0        0     7567 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/pareto_specification.py
--rw-rw-rw-   0        0        0    12630 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/password_requirements.py
--rw-rw-rw-   0        0        0     4087 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/people_stage_lookup.py
--rw-rw-rw-   0        0        0    10847 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/people_stage_system_detail.py
--rw-rw-rw-   0        0        0     8811 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/people_stage_system_summary.py
--rw-rw-rw-   0        0        0     7742 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/per_channel_statistics.py
--rw-rw-rw-   0        0        0     5644 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/per_response_type_per_channel_statistics.py
--rw-rw-rw-   0        0        0     5547 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/per_response_type_statistics.py
--rw-rw-rw-   0        0        0     9905 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/permission.py
--rw-rw-rw-   0        0        0     5893 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/permission_set.py
--rw-rw-rw-   0        0        0     9025 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/process_details.py
--rw-rw-rw-   0        0        0    20923 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/processing_time_statistics.py
--rw-rw-rw-   0        0        0    10870 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/processing_time_statistics_details.py
--rw-rw-rw-   0        0        0     8303 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/purchase_info.py
--rw-rw-rw-   0        0        0     3925 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/query.py
--rw-rw-rw-   0        0        0     4970 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/query_detail_count.py
--rw-rw-rw-   0        0        0     4794 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/query_details.py
--rw-rw-rw-   0        0        0     3471 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/query_file.py
--rw-rw-rw-   0        0        0    12139 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/query_result.py
--rw-rw-rw-   0        0        0    10702 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/range_statistics.py
--rw-rw-rw-   0        0        0     7628 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/record_set.py
--rw-rw-rw-   0        0        0     4579 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/render_data_refresh_job_detail.py
--rw-rw-rw-   0        0        0    10395 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/reset_password_request_detail.py
--rw-rw-rw-   0        0        0     4637 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/resource_category_details.py
--rw-rw-rw-   0        0        0     4637 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/resource_category_summary.py
--rw-rw-rw-   0        0        0     7107 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/resource_details.py
--rw-rw-rw-   0        0        0     7107 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/resource_summary.py
--rw-rw-rw-   0        0        0     6184 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/response_statistics.py
--rw-rw-rw-   0        0        0    17742 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/response_statistics_per_response_type_statistics_map.py
--rw-rw-rw-   0        0        0     6068 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/rfv.py
--rw-rw-rw-   0        0        0     3275 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/rfv_frequency.py
--rw-rw-rw-   0        0        0     6327 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/rfv_recency.py
--rw-rw-rw-   0        0        0     5002 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/rfv_value.py
--rw-rw-rw-   0        0        0     5057 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/row.py
--rw-rw-rw-   0        0        0     3220 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/rule.py
--rw-rw-rw-   0        0        0     4060 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/safe_file_handle.py
--rw-rw-rw-   0        0        0     4263 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/save_query_file.py
--rw-rw-rw-   0        0        0     8445 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/selection.py
--rw-rw-rw-   0        0        0     5159 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/selection_modifiers.py
--rw-rw-rw-   0        0        0    14282 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/selector_variable_info.py
--rw-rw-rw-   0        0        0     5575 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/server_message.py
--rw-rw-rw-   0        0        0     4490 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/session_and_user_details.py
--rw-rw-rw-   0        0        0     7189 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/session_details.py
--rw-rw-rw-   0        0        0    10706 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/share_detail.py
--rw-rw-rw-   0        0        0     9479 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/share_summary.py
--rw-rw-rw-   0        0        0    16541 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/share_update.py
--rw-rw-rw-   0        0        0     4297 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/size.py
--rw-rw-rw-   0        0        0     4669 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/sub_selection.py
--rw-rw-rw-   0        0        0     4732 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/system_lookup.py
--rw-rw-rw-   0        0        0    14408 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/table.py
--rw-rw-rw-   0        0        0     4717 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/table_item.py
--rw-rw-rw-   0        0        0     4202 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/team_detail.py
--rw-rw-rw-   0        0        0     4214 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/team_summary.py
--rw-rw-rw-   0        0        0     5222 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/telemetry_bug_report.py
--rw-rw-rw-   0        0        0    10504 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/telemetry_session.py
--rw-rw-rw-   0        0        0     5751 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/telemetry_state.py
--rw-rw-rw-   0        0        0     3457 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/temporary_file.py
--rw-rw-rw-   0        0        0     6158 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/temporary_file_part.py
--rw-rw-rw-   0        0        0     3783 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/text_variable_info.py
--rw-rw-rw-   0        0        0     8760 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/theme.py
--rw-rw-rw-   0        0        0     3469 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/theme_definition.py
--rw-rw-rw-   0        0        0     5276 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/theme_usage.py
--rw-rw-rw-   0        0        0     4529 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/theme_usage_summary.py
--rw-rw-rw-   0        0        0     3982 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/time_rule.py
--rw-rw-rw-   0        0        0     4560 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/token_login_details.py
--rw-rw-rw-   0        0        0    13261 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/top_n.py
--rw-rw-rw-   0        0        0     3832 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/transfer_audience_ownership_details.py
--rw-rw-rw-   0        0        0     3848 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/transfer_collection_ownership_details.py
--rw-rw-rw-   0        0        0     3403 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/update_team_details.py
--rw-rw-rw-   0        0        0     4652 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/update_telemetry_session_details.py
--rw-rw-rw-   0        0        0     4131 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/update_telemetry_state_details.py
--rw-rw-rw-   0        0        0     5228 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/update_user_details.py
--rw-rw-rw-   0        0        0     7756 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/upsert_collection_detail.py
--rw-rw-rw-   0        0        0    18331 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_audience_composition_detail.py
--rw-rw-rw-   0        0        0    15055 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_audience_composition_summary.py
--rw-rw-rw-   0        0        0    29878 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_audience_detail.py
--rw-rw-rw-   0        0        0    24267 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_audience_summary.py
--rw-rw-rw-   0        0        0    20793 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_collection_detail.py
--rw-rw-rw-   0        0        0    19985 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_collection_summary.py
--rw-rw-rw-   0        0        0     5006 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_configuration_details.py
--rw-rw-rw-   0        0        0    22861 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_dashboard_detail.py
--rw-rw-rw-   0        0        0    19997 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_dashboard_summary.py
--rw-rw-rw-   0        0        0    11073 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_detail.py
--rw-rw-rw-   0        0        0     7275 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_display_details.py
--rw-rw-rw-   0        0        0     7269 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_login.py
--rw-rw-rw-   0        0        0    13116 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_registration_request_detail.py
--rw-rw-rw-   0        0        0    10464 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_registration_request_summary.py
--rw-rw-rw-   0        0        0    10311 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/user_summary.py
--rw-rw-rw-   0        0        0     5169 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/users_lookup.py
--rw-rw-rw-   0        0        0     8023 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/value_rule.py
--rw-rw-rw-   0        0        0     5462 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/var_code.py
--rw-rw-rw-   0        0        0    15026 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/variable.py
--rw-rw-rw-   0        0        0     4515 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/variable_lookup.py
--rw-rw-rw-   0        0        0     3558 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/version_details.py
--rw-rw-rw-   0        0        0     9835 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/visualisation.py
--rw-rw-rw-   0        0        0     4714 2023-06-30 12:18:58.000000 apteco-api-0.3.0/pkg/apteco_api/models/visualisation_detail.py
--rw-rw-rw-   0        0        0    12296 2023-06-30 12:18:59.000000 apteco-api-0.3.0/pkg/apteco_api/rest.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:33:00.914441 apteco-api-0.3.0/pkg/apteco_api.egg-info/
--rw-rw-rw-   0        0        0     9760 2023-06-30 12:33:00.000000 apteco-api-0.3.0/pkg/apteco_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16295 2023-06-30 12:33:00.000000 apteco-api-0.3.0/pkg/apteco_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 12:33:00.000000 apteco-api-0.3.0/pkg/apteco_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-30 12:33:00.000000 apteco-api-0.3.0/pkg/apteco_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 12:33:00.000000 apteco-api-0.3.0/pkg/apteco_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 12:33:01.510775 apteco-api-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 11:46:03.733292 apteco-api-0.3.1/
+-rw-rw-rw-   0        0        0    11556 2019-06-24 15:29:29.000000 apteco-api-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     9760 2023-07-14 11:46:03.732292 apteco-api-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 11:46:03.183290 apteco-api-0.3.1/pkg/
+drwxrwxrwx   0        0        0        0 2023-07-14 11:46:03.192290 apteco-api-0.3.1/pkg/apteco_api/
+-rw-rw-rw-   0        0        0    25109 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:46:03.262291 apteco-api-0.3.1/pkg/apteco_api/api/
+-rw-rw-rw-   0        0        0     2033 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/__init__.py
+-rw-rw-rw-   0        0        0    85079 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/about_api.py
+-rw-rw-rw-   0        0        0    48087 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/audience_compositions_api.py
+-rw-rw-rw-   0        0        0    15326 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/audience_hits_api.py
+-rw-rw-rw-   0        0        0    15768 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/audience_settings_api.py
+-rw-rw-rw-   0        0        0   231588 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/audiences_api.py
+-rw-rw-rw-   0        0        0    15454 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/collection_hits_api.py
+-rw-rw-rw-   0        0        0    80868 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/collections_api.py
+-rw-rw-rw-   0        0        0     8864 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/cubes_api.py
+-rw-rw-rw-   0        0        0   106812 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/dashboards_api.py
+-rw-rw-rw-   0        0        0    72595 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/data_licensing_api.py
+-rw-rw-rw-   0        0        0    45146 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/directories_api.py
+-rw-rw-rw-   0        0        0    23649 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/exports_api.py
+-rw-rw-rw-   0        0        0    13970 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/external_login_api.py
+-rw-rw-rw-   0        0        0    29841 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/fast_stats_builds_api.py
+-rw-rw-rw-   0        0        0    47064 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/fast_stats_jobs_api.py
+-rw-rw-rw-   0        0        0   102470 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/fast_stats_systems_api.py
+-rw-rw-rw-   0        0        0    33501 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/files_api.py
+-rw-rw-rw-   0        0        0    32961 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/groups_api.py
+-rw-rw-rw-   0        0        0   116442 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/people_stage_api.py
+-rw-rw-rw-   0        0        0   107622 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/permissions_api.py
+-rw-rw-rw-   0        0        0    31868 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/queries_api.py
+-rw-rw-rw-   0        0        0    55519 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/sessions_api.py
+-rw-rw-rw-   0        0        0    37597 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/settings_api.py
+-rw-rw-rw-   0        0        0    85237 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/shares_api.py
+-rw-rw-rw-   0        0        0    54038 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/static_resources_api.py
+-rw-rw-rw-   0        0        0    33581 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/teams_api.py
+-rw-rw-rw-   0        0        0    48032 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/telemetry_api.py
+-rw-rw-rw-   0        0        0    29192 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/temporary_files_api.py
+-rw-rw-rw-   0        0        0    36096 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/themes_api.py
+-rw-rw-rw-   0        0        0    28429 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/user_registration_requests_api.py
+-rw-rw-rw-   0        0        0    28956 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/user_reset_password_requests_api.py
+-rw-rw-rw-   0        0        0   145025 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/users_api.py
+-rw-rw-rw-   0        0        0    41797 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api/visualisations_api.py
+-rw-rw-rw-   0        0        0    26203 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/api_client.py
+-rw-rw-rw-   0        0        0    13310 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/configuration.py
+-rw-rw-rw-   0        0        0     3768 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:46:03.731292 apteco-api-0.3.1/pkg/apteco_api/models/
+-rw-rw-rw-   0        0        0    22755 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/models/__init__.py
+-rw-rw-rw-   0        0        0    13413 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/abstract_render_spec.py
+-rw-rw-rw-   0        0        0     8275 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/age_rule.py
+-rw-rw-rw-   0        0        0     7533 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_calculate_job_detail.py
+-rw-rw-rw-   0        0        0     9455 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_check_detail.py
+-rw-rw-rw-   0        0        0     7414 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_check_job_detail.py
+-rw-rw-rw-   0        0        0     7684 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_data_licensing_info_job_detail.py
+-rw-rw-rw-   0        0        0    24859 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_detail.py
+-rw-rw-rw-   0        0        0    15757 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_export_detail.py
+-rw-rw-rw-   0        0        0     7461 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_export_job_detail.py
+-rw-rw-rw-   0        0        0     7304 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_hit_detail.py
+-rw-rw-rw-   0        0        0     6299 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_hit_summary.py
+-rw-rw-rw-   0        0        0     4344 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_query_result.py
+-rw-rw-rw-   0        0        0    12937 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_result_detail.py
+-rw-rw-rw-   0        0        0    10239 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_result_summary.py
+-rw-rw-rw-   0        0        0     7233 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_settings_detail.py
+-rw-rw-rw-   0        0        0     7249 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_settings_summary.py
+-rw-rw-rw-   0        0        0    19344 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_summary.py
+-rw-rw-rw-   0        0        0    14648 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_update_detail.py
+-rw-rw-rw-   0        0        0    10513 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/audience_update_summary.py
+-rw-rw-rw-   0        0        0    12463 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/authorised_permission.py
+-rw-rw-rw-   0        0        0     4673 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/authorised_permission_with_lookups.py
+-rw-rw-rw-   0        0        0     3892 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/authority.py
+-rw-rw-rw-   0        0        0     7220 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/breakpoint.py
+-rw-rw-rw-   0        0        0     3612 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/build_definition.py
+-rw-rw-rw-   0        0        0     7158 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/build_job_detail.py
+-rw-rw-rw-   0        0        0     3571 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/build_result.py
+-rw-rw-rw-   0        0        0     3911 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/calculate_audience_details.py
+-rw-rw-rw-   0        0        0     4828 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/calculate_dashboard_data.py
+-rw-rw-rw-   0        0        0     6419 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/calculate_dashboard_item.py
+-rw-rw-rw-   0        0        0     5340 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/calculate_dashboard_item_job_created_result.py
+-rw-rw-rw-   0        0        0     6532 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/capabilities.py
+-rw-rw-rw-   0        0        0     4838 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/change_password_details.py
+-rw-rw-rw-   0        0        0     7450 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/channel_detail.py
+-rw-rw-rw-   0        0        0     8317 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/channel_statistics.py
+-rw-rw-rw-   0        0        0     7474 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/channel_summary.py
+-rw-rw-rw-   0        0        0     3845 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/check_audience_details.py
+-rw-rw-rw-   0        0        0     5022 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/check_composition_definition.py
+-rw-rw-rw-   0        0        0     7934 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/check_dimension_result.py
+-rw-rw-rw-   0        0        0     4620 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/clause.py
+-rw-rw-rw-   0        0        0    15886 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/collection_detail.py
+-rw-rw-rw-   0        0        0     7398 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/collection_hit_detail.py
+-rw-rw-rw-   0        0        0     6385 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/collection_hit_summary.py
+-rw-rw-rw-   0        0        0     8098 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/collection_part_detail.py
+-rw-rw-rw-   0        0        0     7234 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/collection_part_summary.py
+-rw-rw-rw-   0        0        0    15078 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/collection_summary.py
+-rw-rw-rw-   0        0        0    10066 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/column.py
+-rw-rw-rw-   0        0        0    20298 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/communication_statistics.py
+-rw-rw-rw-   0        0        0    14227 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/composition_detail.py
+-rw-rw-rw-   0        0        0    11029 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/composition_summary.py
+-rw-rw-rw-   0        0        0     4903 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/confirm_reset_password_request.py
+-rw-rw-rw-   0        0        0     4344 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/convert_dashboard_to_audience.py
+-rw-rw-rw-   0        0        0     3534 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/convert_dashboard_to_audience_result.py
+-rw-rw-rw-   0        0        0     3661 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/copy_audience_detail.py
+-rw-rw-rw-   0        0        0     3671 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/copy_dashboard_detail.py
+-rw-rw-rw-   0        0        0     4607 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/count.py
+-rw-rw-rw-   0        0        0     7500 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_audience_composition_detail.py
+-rw-rw-rw-   0        0        0     9647 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_audience_detail.py
+-rw-rw-rw-   0        0        0     3759 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_audience_hit_details.py
+-rw-rw-rw-   0        0        0     9258 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_audience_update.py
+-rw-rw-rw-   0        0        0     3775 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_collection_hit_details.py
+-rw-rw-rw-   0        0        0     8600 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_dashboard_detail.py
+-rw-rw-rw-   0        0        0     9663 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_dashboard_update_detail.py
+-rw-rw-rw-   0        0        0     6102 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_reset_password_request.py
+-rw-rw-rw-   0        0        0     8879 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_session_parameters.py
+-rw-rw-rw-   0        0        0    15507 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_share_detail.py
+-rw-rw-rw-   0        0        0    20708 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_share_update.py
+-rw-rw-rw-   0        0        0     3525 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_team_details.py
+-rw-rw-rw-   0        0        0     6201 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_telemetry_session_details.py
+-rw-rw-rw-   0        0        0     3713 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_telemetry_state_details.py
+-rw-rw-rw-   0        0        0     7229 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_update_theme.py
+-rw-rw-rw-   0        0        0     7918 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_user_details.py
+-rw-rw-rw-   0        0        0     9268 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/create_user_registration_request.py
+-rw-rw-rw-   0        0        0     6843 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/created_share_update_detail.py
+-rw-rw-rw-   0        0        0    10949 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/criteria.py
+-rw-rw-rw-   0        0        0     8225 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/cube.py
+-rw-rw-rw-   0        0        0    13307 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/cube_result.py
+-rw-rw-rw-   0        0        0     4394 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/cube_specification.py
+-rw-rw-rw-   0        0        0     6461 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_content_item.py
+-rw-rw-rw-   0        0        0    14979 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_content_item_detail.py
+-rw-rw-rw-   0        0        0    19161 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_detail.py
+-rw-rw-rw-   0        0        0     3635 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_export_data.py
+-rw-rw-rw-   0        0        0     4591 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_export_data_result.py
+-rw-rw-rw-   0        0        0     9714 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item.py
+-rw-rw-rw-   0        0        0     7181 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_category_display.py
+-rw-rw-rw-   0        0        0     6405 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data.py
+-rw-rw-rw-   0        0        0     5548 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_job_created.py
+-rw-rw-rw-   0        0        0     8532 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_job_detail.py
+-rw-rw-rw-   0        0        0     6117 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_result_detail.py
+-rw-rw-rw-   0        0        0     4716 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_specification.py
+-rw-rw-rw-   0        0        0     8507 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_preview_data.py
+-rw-rw-rw-   0        0        0     3628 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/data_licensing_detail.py
+-rw-rw-rw-   0        0        0     4761 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/data_licensing_system_detail.py
+-rw-rw-rw-   0        0        0     4773 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/data_licensing_system_summary.py
+-rw-rw-rw-   0        0        0     9206 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/data_purchase_detail.py
+-rw-rw-rw-   0        0        0     7349 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/data_purchase_job_detail.py
+-rw-rw-rw-   0        0        0     4445 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/data_view_details.py
+-rw-rw-rw-   0        0        0     3507 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/data_view_summary.py
+-rw-rw-rw-   0        0        0    26245 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/date_rule.py
+-rw-rw-rw-   0        0        0     6616 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/date_settings.py
+-rw-rw-rw-   0        0        0     4046 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/diagram_metadata.py
+-rw-rw-rw-   0        0        0    16094 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dimension.py
+-rw-rw-rw-   0        0        0     5218 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dimension_banding.py
+-rw-rw-rw-   0        0        0     5808 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/dimension_result.py
+-rw-rw-rw-   0        0        0    11353 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/element_detail.py
+-rw-rw-rw-   0        0        0     4375 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/element_key.py
+-rw-rw-rw-   0        0        0    15738 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/element_status.py
+-rw-rw-rw-   0        0        0    11389 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/element_summary.py
+-rw-rw-rw-   0        0        0     6116 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/email_requirements.py
+-rw-rw-rw-   0        0        0    15650 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/endpoint_details.py
+-rw-rw-rw-   0        0        0     5844 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/error_message.py
+-rw-rw-rw-   0        0        0     3920 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/error_message_parameter.py
+-rw-rw-rw-   0        0        0    10554 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/export.py
+-rw-rw-rw-   0        0        0     9405 2023-07-07 12:40:06.000000 apteco-api-0.3.1/pkg/apteco_api/models/export_audience_details.py
+-rw-rw-rw-   0        0        0     4653 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/export_composition_definition.py
+-rw-rw-rw-   0        0        0    11938 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/export_result.py
+-rw-rw-rw-   0        0        0     5630 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/export_system_detail.py
+-rw-rw-rw-   0        0        0     5646 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/export_system_summary.py
+-rw-rw-rw-   0        0        0     8685 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/expression.py
+-rw-rw-rw-   0        0        0     7829 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/fast_stats_system_detail.py
+-rw-rw-rw-   0        0        0     6591 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/fast_stats_system_item.py
+-rw-rw-rw-   0        0        0     6867 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/fast_stats_system_summary.py
+-rw-rw-rw-   0        0        0     5663 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/file_entry.py
+-rw-rw-rw-   0        0        0    10746 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/file_stream.py
+-rw-rw-rw-   0        0        0     3729 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/file_system_summary.py
+-rw-rw-rw-   0        0        0     4389 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/folder.py
+-rw-rw-rw-   0        0        0     4040 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/folder_structure_node.py
+-rw-rw-rw-   0        0        0     4004 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/fraction.py
+-rw-rw-rw-   0        0        0     7564 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/grid_item.py
+-rw-rw-rw-   0        0        0     4218 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/group_detail.py
+-rw-rw-rw-   0        0        0     4230 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/group_summary.py
+-rw-rw-rw-   0        0        0     4513 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/id.py
+-rw-rw-rw-   0        0        0     9065 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/invalid_to_share_user_display_details.py
+-rw-rw-rw-   0        0        0    15996 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/job_detail.py
+-rw-rw-rw-   0        0        0    14284 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/job_summary.py
+-rw-rw-rw-   0        0        0     4187 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/language_details.py
+-rw-rw-rw-   0        0        0     5591 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/last_run_details.py
+-rw-rw-rw-   0        0        0    11076 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/licence.py
+-rw-rw-rw-   0        0        0     7298 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/licensing_info.py
+-rw-rw-rw-   0        0        0     3339 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/licensing_set.py
+-rw-rw-rw-   0        0        0     7535 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/licensing_sets_job_detail.py
+-rw-rw-rw-   0        0        0     7764 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/limits.py
+-rw-rw-rw-   0        0        0     7392 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/link.py
+-rw-rw-rw-   0        0        0     5424 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/list_rule.py
+-rw-rw-rw-   0        0        0     5695 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/logic.py
+-rw-rw-rw-   0        0        0     5038 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/lookups.py
+-rw-rw-rw-   0        0        0    10329 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/measure.py
+-rw-rw-rw-   0        0        0     6220 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/measure_result.py
+-rw-rw-rw-   0        0        0     3441 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/message.py
+-rw-rw-rw-   0        0        0     4647 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/model_property.py
+-rw-rw-rw-   0        0        0     4970 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_items_modify_user_audience.py
+-rw-rw-rw-   0        0        0     5000 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_items_modify_user_collection.py
+-rw-rw-rw-   0        0        0     4985 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_items_modify_user_dashboard.py
+-rw-rw-rw-   0        0        0     6108 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_audience.py
+-rw-rw-rw-   0        0        0     9642 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_audience_detail.py
+-rw-rw-rw-   0        0        0     7502 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_audience_detail_results.py
+-rw-rw-rw-   0        0        0     6188 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_collection.py
+-rw-rw-rw-   0        0        0     6393 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_collection_detail.py
+-rw-rw-rw-   0        0        0     7596 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_collection_detail_results.py
+-rw-rw-rw-   0        0        0     6148 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_dashboard.py
+-rw-rw-rw-   0        0        0    10730 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_dashboard_detail.py
+-rw-rw-rw-   0        0        0     7549 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/modify_user_dashboard_detail_results.py
+-rw-rw-rw-   0        0        0     5038 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/n_per.py
+-rw-rw-rw-   0        0        0     7898 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/notes_alignment.py
+-rw-rw-rw-   0        0        0     7559 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/numeric_variable_info.py
+-rw-rw-rw-   0        0        0     8664 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/output.py
+-rw-rw-rw-   0        0        0     5608 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/output_type.py
+-rw-rw-rw-   0        0        0     6876 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_hit_summary.py
+-rw-rw-rw-   0        0        0     6945 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_result_summary.py
+-rw-rw-rw-   0        0        0     6991 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_settings_summary.py
+-rw-rw-rw-   0        0        0     6807 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_summary.py
+-rw-rw-rw-   0        0        0     6945 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_update_summary.py
+-rw-rw-rw-   0        0        0     7175 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_authorised_permission_with_lookups.py
+-rw-rw-rw-   0        0        0     6784 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_channel_summary.py
+-rw-rw-rw-   0        0        0     6922 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_collection_hit_summary.py
+-rw-rw-rw-   0        0        0     6945 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_collection_part_summary.py
+-rw-rw-rw-   0        0        0     6853 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_collection_summary.py
+-rw-rw-rw-   0        0        0     6876 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_composition_summary.py
+-rw-rw-rw-   0        0        0     7060 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_data_licensing_system_summary.py
+-rw-rw-rw-   0        0        0     6807 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_data_view_summary.py
+-rw-rw-rw-   0        0        0     6761 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_element_status.py
+-rw-rw-rw-   0        0        0     6784 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_element_summary.py
+-rw-rw-rw-   0        0        0     6807 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_endpoint_details.py
+-rw-rw-rw-   0        0        0     6899 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_export_system_summary.py
+-rw-rw-rw-   0        0        0     6899 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_fast_stats_system_item.py
+-rw-rw-rw-   0        0        0     6968 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_fast_stats_system_summary.py
+-rw-rw-rw-   0        0        0     6669 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_file_entry.py
+-rw-rw-rw-   0        0        0     6853 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_file_system_summary.py
+-rw-rw-rw-   0        0        0     6899 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_folder_structure_node.py
+-rw-rw-rw-   0        0        0     6715 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_group_detail.py
+-rw-rw-rw-   0        0        0     6738 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_group_summary.py
+-rw-rw-rw-   0        0        0     6692 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_job_summary.py
+-rw-rw-rw-   0        0        0     6738 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_licensing_set.py
+-rw-rw-rw-   0        0        0     7175 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_modify_user_audience_detail_results.py
+-rw-rw-rw-   0        0        0     7221 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_modify_user_collection_detail_results.py
+-rw-rw-rw-   0        0        0     7198 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_modify_user_dashboard_detail_results.py
+-rw-rw-rw-   0        0        0     7014 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_people_stage_system_summary.py
+-rw-rw-rw-   0        0        0     6991 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_resource_category_summary.py
+-rw-rw-rw-   0        0        0     6807 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_resource_summary.py
+-rw-rw-rw-   0        0        0     6945 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_session_and_user_details.py
+-rw-rw-rw-   0        0        0     6738 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_share_summary.py
+-rw-rw-rw-   0        0        0     6715 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_share_update.py
+-rw-rw-rw-   0        0        0     6577 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_table.py
+-rw-rw-rw-   0        0        0     6715 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_team_summary.py
+-rw-rw-rw-   0        0        0     7152 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_audience_composition_summary.py
+-rw-rw-rw-   0        0        0     6899 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_audience_summary.py
+-rw-rw-rw-   0        0        0     6945 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_collection_summary.py
+-rw-rw-rw-   0        0        0     6922 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_dashboard_summary.py
+-rw-rw-rw-   0        0        0     6876 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_display_details.py
+-rw-rw-rw-   0        0        0     6669 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_login.py
+-rw-rw-rw-   0        0        0     7152 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_registration_request_summary.py
+-rw-rw-rw-   0        0        0     6715 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_summary.py
+-rw-rw-rw-   0        0        0     6623 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_var_code.py
+-rw-rw-rw-   0        0        0     6646 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/paged_results_variable.py
+-rw-rw-rw-   0        0        0     7567 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/pareto_specification.py
+-rw-rw-rw-   0        0        0    12630 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/password_requirements.py
+-rw-rw-rw-   0        0        0     4087 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/people_stage_lookup.py
+-rw-rw-rw-   0        0        0    10847 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/people_stage_system_detail.py
+-rw-rw-rw-   0        0        0     8811 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/people_stage_system_summary.py
+-rw-rw-rw-   0        0        0     7742 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/per_channel_statistics.py
+-rw-rw-rw-   0        0        0     5644 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/per_response_type_per_channel_statistics.py
+-rw-rw-rw-   0        0        0     5547 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/per_response_type_statistics.py
+-rw-rw-rw-   0        0        0     9905 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/permission.py
+-rw-rw-rw-   0        0        0     5893 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/permission_set.py
+-rw-rw-rw-   0        0        0     9025 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/process_details.py
+-rw-rw-rw-   0        0        0    20923 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/processing_time_statistics.py
+-rw-rw-rw-   0        0        0    10870 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/processing_time_statistics_details.py
+-rw-rw-rw-   0        0        0     8303 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/purchase_info.py
+-rw-rw-rw-   0        0        0     3925 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/query.py
+-rw-rw-rw-   0        0        0     4970 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/query_detail_count.py
+-rw-rw-rw-   0        0        0     4794 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/query_details.py
+-rw-rw-rw-   0        0        0     3471 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/query_file.py
+-rw-rw-rw-   0        0        0    12139 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/query_result.py
+-rw-rw-rw-   0        0        0    10702 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/range_statistics.py
+-rw-rw-rw-   0        0        0     7628 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/record_set.py
+-rw-rw-rw-   0        0        0     4579 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/render_data_refresh_job_detail.py
+-rw-rw-rw-   0        0        0    10395 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/reset_password_request_detail.py
+-rw-rw-rw-   0        0        0     4637 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/resource_category_details.py
+-rw-rw-rw-   0        0        0     4637 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/resource_category_summary.py
+-rw-rw-rw-   0        0        0     7107 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/resource_details.py
+-rw-rw-rw-   0        0        0     7107 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/resource_summary.py
+-rw-rw-rw-   0        0        0     6184 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/response_statistics.py
+-rw-rw-rw-   0        0        0    17742 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/response_statistics_per_response_type_statistics_map.py
+-rw-rw-rw-   0        0        0     6068 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/rfv.py
+-rw-rw-rw-   0        0        0     3275 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/rfv_frequency.py
+-rw-rw-rw-   0        0        0     6327 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/rfv_recency.py
+-rw-rw-rw-   0        0        0     5002 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/rfv_value.py
+-rw-rw-rw-   0        0        0     5057 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/row.py
+-rw-rw-rw-   0        0        0     3220 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/rule.py
+-rw-rw-rw-   0        0        0     4060 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/safe_file_handle.py
+-rw-rw-rw-   0        0        0     4263 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/save_query_file.py
+-rw-rw-rw-   0        0        0     8445 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/selection.py
+-rw-rw-rw-   0        0        0     5159 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/selection_modifiers.py
+-rw-rw-rw-   0        0        0    14282 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/selector_variable_info.py
+-rw-rw-rw-   0        0        0     5575 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/server_message.py
+-rw-rw-rw-   0        0        0     4490 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/session_and_user_details.py
+-rw-rw-rw-   0        0        0     7189 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/session_details.py
+-rw-rw-rw-   0        0        0    10706 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/share_detail.py
+-rw-rw-rw-   0        0        0     9479 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/share_summary.py
+-rw-rw-rw-   0        0        0    16541 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/share_update.py
+-rw-rw-rw-   0        0        0     4297 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/size.py
+-rw-rw-rw-   0        0        0     4669 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/sub_selection.py
+-rw-rw-rw-   0        0        0     4732 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/system_lookup.py
+-rw-rw-rw-   0        0        0    14408 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/table.py
+-rw-rw-rw-   0        0        0     4717 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/table_item.py
+-rw-rw-rw-   0        0        0     4202 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/team_detail.py
+-rw-rw-rw-   0        0        0     4214 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/team_summary.py
+-rw-rw-rw-   0        0        0     5222 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/telemetry_bug_report.py
+-rw-rw-rw-   0        0        0    10504 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/telemetry_session.py
+-rw-rw-rw-   0        0        0     5751 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/telemetry_state.py
+-rw-rw-rw-   0        0        0     3457 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/temporary_file.py
+-rw-rw-rw-   0        0        0     6158 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/temporary_file_part.py
+-rw-rw-rw-   0        0        0     3783 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/text_variable_info.py
+-rw-rw-rw-   0        0        0     8760 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/theme.py
+-rw-rw-rw-   0        0        0     3469 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/theme_definition.py
+-rw-rw-rw-   0        0        0     5276 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/theme_usage.py
+-rw-rw-rw-   0        0        0     4529 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/theme_usage_summary.py
+-rw-rw-rw-   0        0        0     3982 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/time_rule.py
+-rw-rw-rw-   0        0        0     4560 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/token_login_details.py
+-rw-rw-rw-   0        0        0    13261 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/top_n.py
+-rw-rw-rw-   0        0        0     3832 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/transfer_audience_ownership_details.py
+-rw-rw-rw-   0        0        0     3848 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/transfer_collection_ownership_details.py
+-rw-rw-rw-   0        0        0     3403 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/update_team_details.py
+-rw-rw-rw-   0        0        0     4652 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/update_telemetry_session_details.py
+-rw-rw-rw-   0        0        0     4131 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/update_telemetry_state_details.py
+-rw-rw-rw-   0        0        0     5228 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/update_user_details.py
+-rw-rw-rw-   0        0        0     7756 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/upsert_collection_detail.py
+-rw-rw-rw-   0        0        0    18331 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_audience_composition_detail.py
+-rw-rw-rw-   0        0        0    15055 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_audience_composition_summary.py
+-rw-rw-rw-   0        0        0    29878 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_audience_detail.py
+-rw-rw-rw-   0        0        0    24267 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_audience_summary.py
+-rw-rw-rw-   0        0        0    20793 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_collection_detail.py
+-rw-rw-rw-   0        0        0    19985 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_collection_summary.py
+-rw-rw-rw-   0        0        0     5006 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_configuration_details.py
+-rw-rw-rw-   0        0        0    22861 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_dashboard_detail.py
+-rw-rw-rw-   0        0        0    19997 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_dashboard_summary.py
+-rw-rw-rw-   0        0        0    11073 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_detail.py
+-rw-rw-rw-   0        0        0     7275 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_display_details.py
+-rw-rw-rw-   0        0        0     7269 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_login.py
+-rw-rw-rw-   0        0        0    13116 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_registration_request_detail.py
+-rw-rw-rw-   0        0        0    10464 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_registration_request_summary.py
+-rw-rw-rw-   0        0        0    10311 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/user_summary.py
+-rw-rw-rw-   0        0        0     5169 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/users_lookup.py
+-rw-rw-rw-   0        0        0     8023 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/value_rule.py
+-rw-rw-rw-   0        0        0     5462 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/var_code.py
+-rw-rw-rw-   0        0        0    15026 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/variable.py
+-rw-rw-rw-   0        0        0     4515 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/variable_lookup.py
+-rw-rw-rw-   0        0        0     3558 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/version_details.py
+-rw-rw-rw-   0        0        0     9835 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/visualisation.py
+-rw-rw-rw-   0        0        0     4714 2023-07-07 12:40:07.000000 apteco-api-0.3.1/pkg/apteco_api/models/visualisation_detail.py
+-rw-rw-rw-   0        0        0    12296 2023-07-07 12:40:08.000000 apteco-api-0.3.1/pkg/apteco_api/rest.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:46:03.198291 apteco-api-0.3.1/pkg/apteco_api.egg-info/
+-rw-rw-rw-   0        0        0     9760 2023-07-14 11:46:02.000000 apteco-api-0.3.1/pkg/apteco_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16295 2023-07-14 11:46:03.000000 apteco-api-0.3.1/pkg/apteco_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 11:46:02.000000 apteco-api-0.3.1/pkg/apteco_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-14 11:46:02.000000 apteco-api-0.3.1/pkg/apteco_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 11:46:02.000000 apteco-api-0.3.1/pkg/apteco_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 11:46:03.733292 apteco-api-0.3.1/setup.cfg
```

### Comparing `apteco-api-0.3.0/LICENSE` & `apteco-api-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/PKG-INFO` & `apteco-api-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apteco-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Apteco API
 Home-page: https://www.apteco.com/
 Author: Apteco Ltd
 Author-email: support@apteco.com
 License: Apache 2.0
 Description: # apteco-api
         A Python wrapper package for the Apteco API to allow access to Apteco Marketing Suite™ resources.
@@ -27,15 +27,15 @@
         
         ## Details
         
         This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
         
         - API version: v2
         - OrbitAPI spec version: 1.9.19.6190
-        - Package version: 0.3.0
+        - Package version: 0.3.1
         - Build package: `org.openapitools.codegen.languages.PythonClientCodegen`
         - Generator version: 4.3.1
         
         
         ## Requirements
         
         - Python 2.7 and 3.4+
```

### Comparing `apteco-api-0.3.0/pkg/apteco_api/__init__.py` & `apteco-api-0.3.1/pkg/apteco_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: support@apteco.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 # import apis into sdk package
 from apteco_api.api.about_api import AboutApi
 from apteco_api.api.audience_compositions_api import AudienceCompositionsApi
 from apteco_api.api.audience_hits_api import AudienceHitsApi
 from apteco_api.api.audience_settings_api import AudienceSettingsApi
 from apteco_api.api.audiences_api import AudiencesApi
```

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/__init__.py` & `apteco-api-0.3.1/pkg/apteco_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/about_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/about_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/audience_compositions_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/audience_compositions_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/audience_hits_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/audience_hits_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/audience_settings_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/audience_settings_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/audiences_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/audiences_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/collection_hits_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/collection_hits_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/collections_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/cubes_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/cubes_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/dashboards_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/dashboards_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/data_licensing_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/data_licensing_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/directories_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/directories_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/exports_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/exports_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/external_login_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/external_login_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/fast_stats_builds_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/fast_stats_builds_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/fast_stats_jobs_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/fast_stats_jobs_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/fast_stats_systems_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/fast_stats_systems_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/files_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/files_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/groups_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/groups_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/people_stage_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/people_stage_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/permissions_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/queries_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/queries_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/sessions_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/settings_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/shares_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/shares_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/static_resources_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/static_resources_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/teams_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/telemetry_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/telemetry_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/temporary_files_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/temporary_files_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/themes_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/user_registration_requests_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/user_registration_requests_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/user_reset_password_requests_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/user_reset_password_requests_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/users_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/users_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api/visualisations_api.py` & `apteco-api-0.3.1/pkg/apteco_api/api/visualisations_api.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/api_client.py` & `apteco-api-0.3.1/pkg/apteco_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.3.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `apteco-api-0.3.0/pkg/apteco_api/configuration.py` & `apteco-api-0.3.1/pkg/apteco_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v2\n"\
-               "SDK Package Version: 0.3.0".\
+               "SDK Package Version: 0.3.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `apteco-api-0.3.0/pkg/apteco_api/exceptions.py` & `apteco-api-0.3.1/pkg/apteco_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/__init__.py` & `apteco-api-0.3.1/pkg/apteco_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/abstract_render_spec.py` & `apteco-api-0.3.1/pkg/apteco_api/models/abstract_render_spec.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/age_rule.py` & `apteco-api-0.3.1/pkg/apteco_api/models/age_rule.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_calculate_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_calculate_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_check_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_check_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_check_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_check_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_data_licensing_info_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_data_licensing_info_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_export_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_export_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_export_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_export_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_hit_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_hit_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_hit_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_hit_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_query_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_query_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_result_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_result_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_result_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_result_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_settings_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_settings_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_settings_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_settings_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_update_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_update_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/audience_update_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/audience_update_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/authorised_permission.py` & `apteco-api-0.3.1/pkg/apteco_api/models/authorised_permission.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/authorised_permission_with_lookups.py` & `apteco-api-0.3.1/pkg/apteco_api/models/authorised_permission_with_lookups.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/authority.py` & `apteco-api-0.3.1/pkg/apteco_api/models/authority.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/breakpoint.py` & `apteco-api-0.3.1/pkg/apteco_api/models/breakpoint.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/build_definition.py` & `apteco-api-0.3.1/pkg/apteco_api/models/build_definition.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/build_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/build_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/build_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/build_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/calculate_audience_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/calculate_audience_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/calculate_dashboard_data.py` & `apteco-api-0.3.1/pkg/apteco_api/models/calculate_dashboard_data.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/calculate_dashboard_item.py` & `apteco-api-0.3.1/pkg/apteco_api/models/calculate_dashboard_item.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/calculate_dashboard_item_job_created_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/calculate_dashboard_item_job_created_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/capabilities.py` & `apteco-api-0.3.1/pkg/apteco_api/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/change_password_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/change_password_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/channel_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/channel_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/channel_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/channel_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/channel_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/channel_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/check_audience_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/check_audience_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/check_composition_definition.py` & `apteco-api-0.3.1/pkg/apteco_api/models/check_composition_definition.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/check_dimension_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/check_dimension_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/clause.py` & `apteco-api-0.3.1/pkg/apteco_api/models/clause.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/collection_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/collection_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/collection_hit_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/collection_hit_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/collection_hit_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/collection_hit_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/collection_part_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/collection_part_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/collection_part_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/collection_part_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/collection_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/collection_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/column.py` & `apteco-api-0.3.1/pkg/apteco_api/models/column.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/communication_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/communication_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/composition_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/composition_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/composition_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/composition_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/confirm_reset_password_request.py` & `apteco-api-0.3.1/pkg/apteco_api/models/confirm_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/convert_dashboard_to_audience.py` & `apteco-api-0.3.1/pkg/apteco_api/models/convert_dashboard_to_audience.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/convert_dashboard_to_audience_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/convert_dashboard_to_audience_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/copy_audience_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/copy_audience_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/copy_dashboard_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/copy_dashboard_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/count.py` & `apteco-api-0.3.1/pkg/apteco_api/models/count.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_audience_composition_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_audience_composition_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_audience_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_audience_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_audience_hit_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_audience_hit_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_audience_update.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_audience_update.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_collection_hit_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_collection_hit_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_dashboard_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_dashboard_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_dashboard_update_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_dashboard_update_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_reset_password_request.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_session_parameters.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_session_parameters.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_share_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_share_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_share_update.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_share_update.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_team_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_team_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_telemetry_session_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_telemetry_session_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_telemetry_state_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_telemetry_state_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_update_theme.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_update_theme.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_user_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_user_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/create_user_registration_request.py` & `apteco-api-0.3.1/pkg/apteco_api/models/create_user_registration_request.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/created_share_update_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/created_share_update_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/criteria.py` & `apteco-api-0.3.1/pkg/apteco_api/models/criteria.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/cube.py` & `apteco-api-0.3.1/pkg/apteco_api/models/cube.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/cube_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/cube_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/cube_specification.py` & `apteco-api-0.3.1/pkg/apteco_api/models/cube_specification.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_content_item.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_content_item.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_content_item_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_content_item_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_export_data.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_export_data.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_export_data_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_export_data_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_category_display.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_category_display.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_job_created.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_job_created.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_result_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_result_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_data_specification.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_data_specification.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dashboard_item_preview_data.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dashboard_item_preview_data.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/data_licensing_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/data_licensing_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/data_licensing_system_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/data_licensing_system_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/data_licensing_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/data_licensing_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/data_purchase_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/data_purchase_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/data_purchase_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/data_purchase_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/data_view_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/data_view_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/data_view_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/data_view_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/date_rule.py` & `apteco-api-0.3.1/pkg/apteco_api/models/date_rule.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/date_settings.py` & `apteco-api-0.3.1/pkg/apteco_api/models/date_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         self._business_year_start_dd = None
         self._business_year_start_mm = None
         self.discriminator = None
 
         self.use_iso8601_week_of_year = use_iso8601_week_of_year
         if business_year_start_dd is not None:
             self.business_year_start_dd = business_year_start_dd
-        self.business_year_start_mm = business_year_start_mm
+        if business_year_start_mm is not None:
+            self.business_year_start_mm = business_year_start_mm
 
     @property
     def use_iso8601_week_of_year(self):
         """Gets the use_iso8601_week_of_year of this DateSettings.  # noqa: E501
 
         Whether the FastStats system uses ISO 8601 date and time format  # noqa: E501
 
@@ -125,16 +126,14 @@
         """Sets the business_year_start_mm of this DateSettings.
 
         If defined, the month of the ywear that the \"Business year\" starts on.  For example, the UK tax year  starts on the 6th April, so this property would have a value of 4.  # noqa: E501
 
         :param business_year_start_mm: The business_year_start_mm of this DateSettings.  # noqa: E501
         :type: int
         """
-        if self.local_vars_configuration.client_side_validation and business_year_start_mm is None:  # noqa: E501
-            raise ValueError("Invalid value for `business_year_start_mm`, must not be `None`")  # noqa: E501
 
         self._business_year_start_mm = business_year_start_mm
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/diagram_metadata.py` & `apteco-api-0.3.1/pkg/apteco_api/models/diagram_metadata.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dimension.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dimension.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dimension_banding.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dimension_banding.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/dimension_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/dimension_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/element_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/element_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/element_key.py` & `apteco-api-0.3.1/pkg/apteco_api/models/element_key.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/element_status.py` & `apteco-api-0.3.1/pkg/apteco_api/models/element_status.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/element_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/element_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/email_requirements.py` & `apteco-api-0.3.1/pkg/apteco_api/models/email_requirements.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/endpoint_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/error_message.py` & `apteco-api-0.3.1/pkg/apteco_api/models/error_message.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/error_message_parameter.py` & `apteco-api-0.3.1/pkg/apteco_api/models/error_message_parameter.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/export.py` & `apteco-api-0.3.1/pkg/apteco_api/models/export.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/export_audience_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/export_audience_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/export_composition_definition.py` & `apteco-api-0.3.1/pkg/apteco_api/models/export_composition_definition.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/export_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/export_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/export_system_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/export_system_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/export_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/export_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/expression.py` & `apteco-api-0.3.1/pkg/apteco_api/models/expression.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/fast_stats_system_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/fast_stats_system_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/fast_stats_system_item.py` & `apteco-api-0.3.1/pkg/apteco_api/models/fast_stats_system_item.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/fast_stats_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/fast_stats_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/file_entry.py` & `apteco-api-0.3.1/pkg/apteco_api/models/file_entry.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/file_stream.py` & `apteco-api-0.3.1/pkg/apteco_api/models/file_stream.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/file_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/file_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/folder.py` & `apteco-api-0.3.1/pkg/apteco_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/folder_structure_node.py` & `apteco-api-0.3.1/pkg/apteco_api/models/folder_structure_node.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/fraction.py` & `apteco-api-0.3.1/pkg/apteco_api/models/fraction.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/grid_item.py` & `apteco-api-0.3.1/pkg/apteco_api/models/grid_item.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/group_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/group_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/group_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/group_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/id.py` & `apteco-api-0.3.1/pkg/apteco_api/models/id.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/invalid_to_share_user_display_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/invalid_to_share_user_display_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/job_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/job_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/language_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/language_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/last_run_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/last_run_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/licence.py` & `apteco-api-0.3.1/pkg/apteco_api/models/licence.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/licensing_info.py` & `apteco-api-0.3.1/pkg/apteco_api/models/licensing_info.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/licensing_set.py` & `apteco-api-0.3.1/pkg/apteco_api/models/licensing_set.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/licensing_sets_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/licensing_sets_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/limits.py` & `apteco-api-0.3.1/pkg/apteco_api/models/limits.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/link.py` & `apteco-api-0.3.1/pkg/apteco_api/models/link.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/list_rule.py` & `apteco-api-0.3.1/pkg/apteco_api/models/list_rule.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/logic.py` & `apteco-api-0.3.1/pkg/apteco_api/models/logic.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/lookups.py` & `apteco-api-0.3.1/pkg/apteco_api/models/lookups.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/measure.py` & `apteco-api-0.3.1/pkg/apteco_api/models/measure.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/measure_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/measure_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/message.py` & `apteco-api-0.3.1/pkg/apteco_api/models/message.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/model_property.py` & `apteco-api-0.3.1/pkg/apteco_api/models/model_property.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_items_modify_user_audience.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_items_modify_user_audience.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_items_modify_user_collection.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_items_modify_user_collection.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_items_modify_user_dashboard.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_items_modify_user_dashboard.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_audience.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_audience.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_audience_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_audience_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_audience_detail_results.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_audience_detail_results.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_collection.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_collection.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_collection_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_collection_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_collection_detail_results.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_collection_detail_results.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_dashboard.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_dashboard.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_dashboard_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_dashboard_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/modify_user_dashboard_detail_results.py` & `apteco-api-0.3.1/pkg/apteco_api/models/modify_user_dashboard_detail_results.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/n_per.py` & `apteco-api-0.3.1/pkg/apteco_api/models/n_per.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/notes_alignment.py` & `apteco-api-0.3.1/pkg/apteco_api/models/notes_alignment.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/numeric_variable_info.py` & `apteco-api-0.3.1/pkg/apteco_api/models/numeric_variable_info.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/output.py` & `apteco-api-0.3.1/pkg/apteco_api/models/output.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/output_type.py` & `apteco-api-0.3.1/pkg/apteco_api/models/output_type.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_hit_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_hit_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_result_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_result_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_settings_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_settings_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_audience_update_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_audience_update_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_authorised_permission_with_lookups.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_authorised_permission_with_lookups.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_channel_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_channel_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_collection_hit_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_collection_hit_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_collection_part_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_collection_part_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_collection_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_collection_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_composition_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_composition_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_data_licensing_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_data_licensing_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_data_view_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_data_view_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_element_status.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_element_status.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_element_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_element_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_endpoint_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_endpoint_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_export_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_export_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_fast_stats_system_item.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_fast_stats_system_item.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_fast_stats_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_fast_stats_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_file_entry.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_file_entry.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_file_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_file_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_folder_structure_node.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_folder_structure_node.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_group_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_group_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_group_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_group_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_job_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_job_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_licensing_set.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_licensing_set.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_modify_user_audience_detail_results.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_modify_user_audience_detail_results.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_modify_user_collection_detail_results.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_modify_user_collection_detail_results.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_modify_user_dashboard_detail_results.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_modify_user_dashboard_detail_results.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_people_stage_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_people_stage_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_resource_category_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_resource_category_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_resource_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_resource_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_session_and_user_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_session_and_user_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_share_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_share_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_share_update.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_share_update.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_table.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_table.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_team_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_team_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_audience_composition_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_audience_composition_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_audience_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_audience_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_collection_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_collection_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_dashboard_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_dashboard_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_display_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_display_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_login.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_login.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_registration_request_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_registration_request_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_user_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_user_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_var_code.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_var_code.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/paged_results_variable.py` & `apteco-api-0.3.1/pkg/apteco_api/models/paged_results_variable.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/pareto_specification.py` & `apteco-api-0.3.1/pkg/apteco_api/models/pareto_specification.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/password_requirements.py` & `apteco-api-0.3.1/pkg/apteco_api/models/password_requirements.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/people_stage_lookup.py` & `apteco-api-0.3.1/pkg/apteco_api/models/people_stage_lookup.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/people_stage_system_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/people_stage_system_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/people_stage_system_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/people_stage_system_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/per_channel_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/per_channel_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/per_response_type_per_channel_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/per_response_type_per_channel_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/per_response_type_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/per_response_type_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/permission.py` & `apteco-api-0.3.1/pkg/apteco_api/models/permission.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/permission_set.py` & `apteco-api-0.3.1/pkg/apteco_api/models/permission_set.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/process_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/process_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/processing_time_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/processing_time_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/processing_time_statistics_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/processing_time_statistics_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/purchase_info.py` & `apteco-api-0.3.1/pkg/apteco_api/models/purchase_info.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/query.py` & `apteco-api-0.3.1/pkg/apteco_api/models/query.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/query_detail_count.py` & `apteco-api-0.3.1/pkg/apteco_api/models/query_detail_count.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/query_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/query_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/query_file.py` & `apteco-api-0.3.1/pkg/apteco_api/models/query_file.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/query_result.py` & `apteco-api-0.3.1/pkg/apteco_api/models/query_result.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/range_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/range_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/record_set.py` & `apteco-api-0.3.1/pkg/apteco_api/models/record_set.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/render_data_refresh_job_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/render_data_refresh_job_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/reset_password_request_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/reset_password_request_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/resource_category_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/resource_category_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/resource_category_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/resource_category_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/resource_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/resource_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/resource_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/resource_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/response_statistics.py` & `apteco-api-0.3.1/pkg/apteco_api/models/response_statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/response_statistics_per_response_type_statistics_map.py` & `apteco-api-0.3.1/pkg/apteco_api/models/response_statistics_per_response_type_statistics_map.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/rfv.py` & `apteco-api-0.3.1/pkg/apteco_api/models/rfv.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/rfv_frequency.py` & `apteco-api-0.3.1/pkg/apteco_api/models/rfv_frequency.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/rfv_recency.py` & `apteco-api-0.3.1/pkg/apteco_api/models/rfv_recency.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/rfv_value.py` & `apteco-api-0.3.1/pkg/apteco_api/models/rfv_value.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/row.py` & `apteco-api-0.3.1/pkg/apteco_api/models/row.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/rule.py` & `apteco-api-0.3.1/pkg/apteco_api/models/rule.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/safe_file_handle.py` & `apteco-api-0.3.1/pkg/apteco_api/models/safe_file_handle.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/save_query_file.py` & `apteco-api-0.3.1/pkg/apteco_api/models/save_query_file.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/selection.py` & `apteco-api-0.3.1/pkg/apteco_api/models/selection.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/selection_modifiers.py` & `apteco-api-0.3.1/pkg/apteco_api/models/selection_modifiers.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/selector_variable_info.py` & `apteco-api-0.3.1/pkg/apteco_api/models/selector_variable_info.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/server_message.py` & `apteco-api-0.3.1/pkg/apteco_api/models/server_message.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/session_and_user_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/session_and_user_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/session_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/session_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/share_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/share_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/share_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/share_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/share_update.py` & `apteco-api-0.3.1/pkg/apteco_api/models/share_update.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/size.py` & `apteco-api-0.3.1/pkg/apteco_api/models/size.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/sub_selection.py` & `apteco-api-0.3.1/pkg/apteco_api/models/sub_selection.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/system_lookup.py` & `apteco-api-0.3.1/pkg/apteco_api/models/system_lookup.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/table.py` & `apteco-api-0.3.1/pkg/apteco_api/models/table.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/table_item.py` & `apteco-api-0.3.1/pkg/apteco_api/models/table_item.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/team_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/team_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/team_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/team_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/telemetry_bug_report.py` & `apteco-api-0.3.1/pkg/apteco_api/models/telemetry_bug_report.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/telemetry_session.py` & `apteco-api-0.3.1/pkg/apteco_api/models/telemetry_session.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/telemetry_state.py` & `apteco-api-0.3.1/pkg/apteco_api/models/telemetry_state.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/temporary_file.py` & `apteco-api-0.3.1/pkg/apteco_api/models/temporary_file.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/temporary_file_part.py` & `apteco-api-0.3.1/pkg/apteco_api/models/temporary_file_part.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/text_variable_info.py` & `apteco-api-0.3.1/pkg/apteco_api/models/text_variable_info.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/theme.py` & `apteco-api-0.3.1/pkg/apteco_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/theme_definition.py` & `apteco-api-0.3.1/pkg/apteco_api/models/theme_definition.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/theme_usage.py` & `apteco-api-0.3.1/pkg/apteco_api/models/theme_usage.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/theme_usage_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/theme_usage_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/time_rule.py` & `apteco-api-0.3.1/pkg/apteco_api/models/time_rule.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/token_login_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/token_login_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/top_n.py` & `apteco-api-0.3.1/pkg/apteco_api/models/top_n.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/transfer_audience_ownership_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/transfer_audience_ownership_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/transfer_collection_ownership_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/transfer_collection_ownership_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/update_team_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/update_team_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/update_telemetry_session_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/update_telemetry_session_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/update_telemetry_state_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/update_telemetry_state_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/update_user_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/update_user_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/upsert_collection_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/upsert_collection_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_audience_composition_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_audience_composition_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_audience_composition_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_audience_composition_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_audience_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_audience_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_audience_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_audience_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_collection_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_collection_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_collection_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_collection_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_configuration_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_configuration_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_dashboard_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_dashboard_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_dashboard_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_dashboard_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_display_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_display_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_login.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_login.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_registration_request_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_registration_request_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_registration_request_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_registration_request_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/user_summary.py` & `apteco-api-0.3.1/pkg/apteco_api/models/user_summary.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/users_lookup.py` & `apteco-api-0.3.1/pkg/apteco_api/models/users_lookup.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/value_rule.py` & `apteco-api-0.3.1/pkg/apteco_api/models/value_rule.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/var_code.py` & `apteco-api-0.3.1/pkg/apteco_api/models/var_code.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/variable.py` & `apteco-api-0.3.1/pkg/apteco_api/models/variable.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/variable_lookup.py` & `apteco-api-0.3.1/pkg/apteco_api/models/variable_lookup.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/version_details.py` & `apteco-api-0.3.1/pkg/apteco_api/models/version_details.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/visualisation.py` & `apteco-api-0.3.1/pkg/apteco_api/models/visualisation.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/models/visualisation_detail.py` & `apteco-api-0.3.1/pkg/apteco_api/models/visualisation_detail.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api/rest.py` & `apteco-api-0.3.1/pkg/apteco_api/rest.py`

 * *Files identical despite different names*

### Comparing `apteco-api-0.3.0/pkg/apteco_api.egg-info/PKG-INFO` & `apteco-api-0.3.1/pkg/apteco_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apteco-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Apteco API
 Home-page: https://www.apteco.com/
 Author: Apteco Ltd
 Author-email: support@apteco.com
 License: Apache 2.0
 Description: # apteco-api
         A Python wrapper package for the Apteco API to allow access to Apteco Marketing Suite™ resources.
@@ -27,15 +27,15 @@
         
         ## Details
         
         This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
         
         - API version: v2
         - OrbitAPI spec version: 1.9.19.6190
-        - Package version: 0.3.0
+        - Package version: 0.3.1
         - Build package: `org.openapitools.codegen.languages.PythonClientCodegen`
         - Generator version: 4.3.1
         
         
         ## Requirements
         
         - Python 2.7 and 3.4+
```

### Comparing `apteco-api-0.3.0/pkg/apteco_api.egg-info/SOURCES.txt` & `apteco-api-0.3.1/pkg/apteco_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

