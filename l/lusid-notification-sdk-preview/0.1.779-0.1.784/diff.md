# Comparing `tmp/lusid-notification-sdk-preview-0.1.779.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.784.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.779.tar", last modified: Mon Jul 10 16:43:08 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.784.tar", last modified: Fri Jul 14 10:29:19 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.779.tar` & `lusid-notification-sdk-preview-0.1.784.tar`

### file list

```diff
@@ -1,64 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7868 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4184 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27783 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     2896 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11055 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10618 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    13061 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15029 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     9778 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6879 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)    33426 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8104 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8447 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12181 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15899 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2559 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 16:43:08.000000 lusid-notification-sdk-preview-0.1.779/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-07-10 16:42:32.000000 lusid-notification-sdk-preview-0.1.779/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8236 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27783 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11055 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     8318 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    10618 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    13061 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15029 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/email_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6879 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    33958 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    24077 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8104 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6008 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/sms_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8447 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12181 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15899 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13098 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/models/webhook_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 10:29:19.000000 lusid-notification-sdk-preview-0.1.784/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-14 10:28:41.000000 lusid-notification-sdk-preview-0.1.784/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.779/README.md` & `lusid-notification-sdk-preview-0.1.784/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.779
-- Package version: 0.1.779
+- API version: 0.1.784
+- Package version: 0.1.784
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -109,17 +109,19 @@
 
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
+ - [AmazonSqsNotificationTypeResponse](docs/AmazonSqsNotificationTypeResponse.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
+ - [EmailNotificationTypeResponse](docs/EmailNotificationTypeResponse.md)
  - [EventFieldDefinition](docs/EventFieldDefinition.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
@@ -127,24 +129,27 @@
  - [ManualEventBody](docs/ManualEventBody.md)
  - [ManualEventHeader](docs/ManualEventHeader.md)
  - [ManualEventRequest](docs/ManualEventRequest.md)
  - [MatchingPattern](docs/MatchingPattern.md)
  - [Notification](docs/Notification.md)
  - [NotificationStatus](docs/NotificationStatus.md)
  - [NotificationType](docs/NotificationType.md)
+ - [NotificationTypeResponse](docs/NotificationTypeResponse.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [ResourceListOfEventTypeSchema](docs/ResourceListOfEventTypeSchema.md)
  - [ResourceListOfNotification](docs/ResourceListOfNotification.md)
  - [ResourceListOfSubscription](docs/ResourceListOfSubscription.md)
  - [SmsNotificationType](docs/SmsNotificationType.md)
+ - [SmsNotificationTypeResponse](docs/SmsNotificationTypeResponse.md)
  - [Subscription](docs/Subscription.md)
  - [UpdateNotificationRequest](docs/UpdateNotificationRequest.md)
  - [UpdateSubscription](docs/UpdateSubscription.md)
  - [WebhookNotificationType](docs/WebhookNotificationType.md)
+ - [WebhookNotificationTypeResponse](docs/WebhookNotificationTypeResponse.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
 Authentication schemes defined for the API:
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.779"
+__version__ = "0.1.784"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
@@ -33,17 +33,19 @@
 from lusid_notification.exceptions import ApiKeyError
 from lusid_notification.exceptions import ApiException
 # import models into sdk package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
+from lusid_notification.models.amazon_sqs_notification_type_response import AmazonSqsNotificationTypeResponse
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
+from lusid_notification.models.email_notification_type_response import EmailNotificationTypeResponse
 from lusid_notification.models.event_field_definition import EventFieldDefinition
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
@@ -51,24 +53,27 @@
 from lusid_notification.models.manual_event_body import ManualEventBody
 from lusid_notification.models.manual_event_header import ManualEventHeader
 from lusid_notification.models.manual_event_request import ManualEventRequest
 from lusid_notification.models.matching_pattern import MatchingPattern
 from lusid_notification.models.notification import Notification
 from lusid_notification.models.notification_status import NotificationStatus
 from lusid_notification.models.notification_type import NotificationType
+from lusid_notification.models.notification_type_response import NotificationTypeResponse
 from lusid_notification.models.resource_id import ResourceId
 from lusid_notification.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_notification.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notification.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notification.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notification.models.sms_notification_type import SmsNotificationType
+from lusid_notification.models.sms_notification_type_response import SmsNotificationTypeResponse
 from lusid_notification.models.subscription import Subscription
 from lusid_notification.models.update_notification_request import UpdateNotificationRequest
 from lusid_notification.models.update_subscription import UpdateSubscription
 from lusid_notification.models.webhook_notification_type import WebhookNotificationType
+from lusid_notification.models.webhook_notification_type_response import WebhookNotificationTypeResponse
 
 # import utilities into sdk package
 from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
 from fbnsdkutilities.utilities.api_configuration import ApiConfiguration
 from fbnsdkutilities.utilities.api_configuration_loader import ApiConfigurationLoader
 from fbnsdkutilities.utilities.refreshing_token import RefreshingToken
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/api/manual_event_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.779'
+        header_params['X-LUSID-SDK-Version'] = '0.1.784'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.779/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.784/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.779\n"\
-               "SDK Package Version: 0.1.779".\
+               "Version of the API: 0.1.784\n"\
+               "SDK Package Version: 0.1.784".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/create_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/event_field_definition.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/event_field_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/manual_event_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/notification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,15 +38,15 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'notification_id': 'str',
         'display_name': 'str',
         'description': 'str',
-        'notification_type': 'object',
+        'notification_type': 'NotificationTypeResponse',
         'created_at': 'datetime',
         'user_id_created': 'str',
         'modified_at': 'datetime',
         'user_id_modified': 'str',
         'href': 'str'
     }
 
@@ -79,16 +79,16 @@
         
         :param notification_id:  The identifier of the notification (required)
         :type notification_id: str
         :param display_name:  The name of the notification (required)
         :type display_name: str
         :param description:  The summary of the services provided by the notification
         :type description: str
-        :param notification_type:  The type and contents of the notification (required)
-        :type notification_type: object
+        :param notification_type:  (required)
+        :type notification_type: lusid_notification.NotificationTypeResponse
         :param created_at:  The time at which the subscription was made (required)
         :type created_at: datetime
         :param user_id_created:  The user who made the subscription (required)
         :type user_id_created: str
         :param modified_at:  The time at which the subscription was last modified (required)
         :type modified_at: datetime
         :param user_id_modified:  The user who last modified the subscription (required)
@@ -216,30 +216,30 @@
 
         self._description = description
 
     @property
     def notification_type(self):
         """Gets the notification_type of this Notification.  # noqa: E501
 
-        The type and contents of the notification  # noqa: E501
 
         :return: The notification_type of this Notification.  # noqa: E501
-        :rtype: object
+        :rtype: lusid_notification.NotificationTypeResponse
         """
         return self._notification_type
 
     @notification_type.setter
     def notification_type(self, notification_type):
         """Sets the notification_type of this Notification.
 
-        The type and contents of the notification  # noqa: E501
 
         :param notification_type: The notification_type of this Notification.  # noqa: E501
-        :type notification_type: object
+        :type notification_type: lusid_notification.NotificationTypeResponse
         """
+        if self.local_vars_configuration.client_side_validation and notification_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `notification_type`, must not be `None`")  # noqa: E501
 
         self._notification_type = notification_type
 
     @property
     def created_at(self):
         """Gets the created_at of this Notification.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/notification_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/notification_type.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -77,15 +77,15 @@
         'authentication_type': 'authenticationType',
         'authentication_configuration_item_paths': 'authenticationConfigurationItemPaths',
         'content_type': 'contentType',
         'content': 'content'
     }
 
     required_map = {
-        'type': 'optional',
+        'type': 'required',
         'api_key_ref': 'required',
         'api_secret_ref': 'required',
         'body': 'required',
         'queue_url_ref': 'required',
         'subject': 'required',
         'plain_text_body': 'required',
         'html_body': 'optional',
@@ -100,15 +100,15 @@
         'content_type': 'required',
         'content': 'optional'
     }
 
     def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
         """NotificationType - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification
+        :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store (required)
         :type api_secret_ref: str
         :param body:  The body of the SMS (required)
         :type body: str
@@ -201,14 +201,22 @@
         """Sets the type of this NotificationType.
 
         The type of delivery mechanism for this notification  # noqa: E501
 
         :param type: The type of this NotificationType.  # noqa: E501
         :type type: str
         """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        allowed_values = ["Webhook"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
         self._type = type
 
     @property
     def api_key_ref(self):
         """Gets the api_key_ref of this NotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/sms_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/update_notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.779
+    The version of the OpenAPI document: 0.1.784
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.784/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.779/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.784/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 lusid_notification/api/notifications_api.py
 lusid_notification/api/subscriptions_api.py
 lusid_notification/models/__init__.py
 lusid_notification/models/access_controlled_action.py
 lusid_notification/models/access_controlled_resource.py
 lusid_notification/models/action_id.py
 lusid_notification/models/amazon_sqs_notification_type.py
+lusid_notification/models/amazon_sqs_notification_type_response.py
 lusid_notification/models/create_notification_request.py
 lusid_notification/models/create_subscription.py
 lusid_notification/models/email_notification_type.py
+lusid_notification/models/email_notification_type_response.py
 lusid_notification/models/event_field_definition.py
 lusid_notification/models/event_type_schema.py
 lusid_notification/models/id_selector_definition.py
 lusid_notification/models/identifier_part_schema.py
 lusid_notification/models/link.py
 lusid_notification/models/lusid_problem_details.py
 lusid_notification/models/lusid_validation_problem_details.py
@@ -32,24 +34,27 @@
 lusid_notification/models/manual_event_body.py
 lusid_notification/models/manual_event_header.py
 lusid_notification/models/manual_event_request.py
 lusid_notification/models/matching_pattern.py
 lusid_notification/models/notification.py
 lusid_notification/models/notification_status.py
 lusid_notification/models/notification_type.py
+lusid_notification/models/notification_type_response.py
 lusid_notification/models/resource_id.py
 lusid_notification/models/resource_list_of_access_controlled_resource.py
 lusid_notification/models/resource_list_of_event_type_schema.py
 lusid_notification/models/resource_list_of_notification.py
 lusid_notification/models/resource_list_of_subscription.py
 lusid_notification/models/sms_notification_type.py
+lusid_notification/models/sms_notification_type_response.py
 lusid_notification/models/subscription.py
 lusid_notification/models/update_notification_request.py
 lusid_notification/models/update_subscription.py
 lusid_notification/models/webhook_notification_type.py
+lusid_notification/models/webhook_notification_type_response.py
 lusid_notification/utilities/__init__.py
 lusid_notification/utilities/config_keys.json
 lusid_notification/utilities/config_keys.py
 lusid_notification_sdk_preview.egg-info/PKG-INFO
 lusid_notification_sdk_preview.egg-info/SOURCES.txt
 lusid_notification_sdk_preview.egg-info/dependency_links.txt
 lusid_notification_sdk_preview.egg-info/requires.txt
```

### Comparing `lusid-notification-sdk-preview-0.1.779/setup.py` & `lusid-notification-sdk-preview-0.1.784/setup.py`

 * *Files identical despite different names*

