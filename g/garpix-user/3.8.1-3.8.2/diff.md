# Comparing `tmp/garpix_user-3.8.1.tar.gz` & `tmp/garpix_user-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_user-3.8.1.tar", last modified: Mon Jun 26 12:00:42 2023, max compression
+gzip compressed data, was "garpix_user-3.8.2.tar", last modified: Fri Jul 14 08:28:18 2023, max compression
```

## Comparing `garpix_user-3.8.1.tar` & `garpix_user-3.8.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.815034 garpix_user-3.8.1/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-06-26 12:00:42.000000 garpix_user-3.8.1/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-06-26 12:00:42.814795 garpix_user-3.8.1/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.805172 garpix_user-3.8.1/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5614 2023-06-26 12:00:32.000000 garpix_user-3.8.1/garpix_user/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.8.1/garpix_user/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10758 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.8.1/garpix_user/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806377 garpix_user-3.8.1/garpix_user/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/admin/referral_type.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.8.1/garpix_user/admin/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/admin/user_session.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.8.1/garpix_user/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.8.1/garpix_user/exceptions.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806587 garpix_user-3.8.1/garpix_user/forms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/forms/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1009 2023-05-31 03:44:48.000000 garpix_user-3.8.1/garpix_user/forms/login.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.802440 garpix_user-3.8.1/garpix_user/locale/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.802491 garpix_user-3.8.1/garpix_user/locale/ru/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806815 garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7137 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9522 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806926 garpix_user-3.8.1/garpix_user/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.807106 garpix_user-3.8.1/garpix_user/mixins/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/mixins/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.808653 garpix_user-3.8.1/garpix_user/mixins/models/confirm/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/code_length_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5477 2023-05-10 13:07:30.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/email_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3562 2023-05-10 13:07:30.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/phone_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5552 2023-06-26 12:00:32.000000 garpix_user-3.8.1/garpix_user/mixins/models/restore_password.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.809071 garpix_user-3.8.1/garpix_user/mixins/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/mixins/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.8.1/garpix_user/mixins/serializers/password_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.8.1/garpix_user/mixins/serializers/to_lower.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.809809 garpix_user-3.8.1/garpix_user/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.8.1/garpix_user/models/access_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/models/refferal.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.8.1/garpix_user/models/refresh_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.8.1/garpix_user/models/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4986 2023-04-24 07:29:27.000000 garpix_user-3.8.1/garpix_user/models/user_session.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.810002 garpix_user-3.8.1/garpix_user/rest/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/rest/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2702 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/rest/authentication.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.810956 garpix_user-3.8.1/garpix_user/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      820 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.8.1/garpix_user/serializers/auth_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/serializers/email_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      247 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/serializers/jwt_data_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1584 2023-05-31 09:44:39.000000 garpix_user-3.8.1/garpix_user/serializers/passwrod_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/serializers/phone_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/serializers/refresh_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.8.1/garpix_user/serializers/registration_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.8.1/garpix_user/serializers/user_session_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-26 12:00:32.000000 garpix_user-3.8.1/garpix_user/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.811184 garpix_user-3.8.1/garpix_user/tasks/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.8.1/garpix_user/tasks/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.8.1/garpix_user/tasks/delete_unconfirmed_users.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.803145 garpix_user-3.8.1/garpix_user/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.811293 garpix_user-3.8.1/garpix_user/templates/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/templates/garpix_user/send_confirm.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.811515 garpix_user-3.8.1/garpix_user/tests/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.812014 garpix_user-3.8.1/garpix_user/tests/test_api/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/test_api/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.812240 garpix_user-3.8.1/garpix_user/tests/test_api/_trial_temp/
--rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/tests/test_api/_trial_temp/_trial_marker
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.8.1/garpix_user/tests/test_api/_trial_temp/test.log
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/test_api/api_login.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/tests/test_api/api_registration.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.8.1/garpix_user/tests/test_api/api_user_session_restore_password.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/tests/test_views.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.812606 garpix_user-3.8.1/garpix_user/tests/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/utils/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/utils/test_case_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2661 2023-06-21 15:22:29.000000 garpix_user-3.8.1/garpix_user/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.813293 garpix_user-3.8.1/garpix_user/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-06-22 15:00:39.000000 garpix_user-3.8.1/garpix_user/utils/backends.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/utils/current_date.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.8.1/garpix_user/utils/drf_spectacular.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      329 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/utils/get_token_from_request.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.8.1/garpix_user/utils/repluralize.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.814594 garpix_user-3.8.1/garpix_user/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/change_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.8.1/garpix_user/views/email_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2426 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/views/login_views.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/views/logout_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2942 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/views/obtain_auth_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.8.1/garpix_user/views/phone_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/referral_links_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.8.1/garpix_user/views/refresh_token_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/registration_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3452 2023-05-31 09:44:39.000000 garpix_user-3.8.1/garpix_user/views/restore_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/user_session_view.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.805906 garpix_user-3.8.1/garpix_user.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3187 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      279 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-26 12:00:42.815072 garpix_user-3.8.1/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-26 12:00:42.000000 garpix_user-3.8.1/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.330601 garpix_user-3.8.2/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-07-14 08:28:18.000000 garpix_user-3.8.2/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-07-14 08:28:18.330376 garpix_user-3.8.2/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.320161 garpix_user-3.8.2/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5675 2023-07-14 08:27:10.000000 garpix_user-3.8.2/garpix_user/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.8.2/garpix_user/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10758 2023-06-23 07:44:40.000000 garpix_user-3.8.2/garpix_user/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.8.2/garpix_user/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.321316 garpix_user-3.8.2/garpix_user/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/admin/referral_type.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.8.2/garpix_user/admin/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/admin/user_session.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.8.2/garpix_user/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2124 2023-07-14 08:25:58.000000 garpix_user-3.8.2/garpix_user/exceptions.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.321538 garpix_user-3.8.2/garpix_user/forms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/forms/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1009 2023-05-31 03:44:48.000000 garpix_user-3.8.2/garpix_user/forms/login.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.286001 garpix_user-3.8.2/garpix_user/locale/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.286044 garpix_user-3.8.2/garpix_user/locale/ru/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.321774 garpix_user-3.8.2/garpix_user/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7198 2023-07-14 08:14:46.000000 garpix_user-3.8.2/garpix_user/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9585 2023-07-14 08:15:37.000000 garpix_user-3.8.2/garpix_user/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.321892 garpix_user-3.8.2/garpix_user/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.322106 garpix_user-3.8.2/garpix_user/mixins/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/mixins/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.322596 garpix_user-3.8.2/garpix_user/mixins/models/confirm/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/mixins/models/confirm/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.8.2/garpix_user/mixins/models/confirm/code_length_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5477 2023-05-10 13:07:30.000000 garpix_user-3.8.2/garpix_user/mixins/models/confirm/email_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3562 2023-05-10 13:07:30.000000 garpix_user-3.8.2/garpix_user/mixins/models/confirm/phone_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5552 2023-06-26 12:00:32.000000 garpix_user-3.8.2/garpix_user/mixins/models/restore_password.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.323293 garpix_user-3.8.2/garpix_user/mixins/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/mixins/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.8.2/garpix_user/mixins/serializers/password_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.8.2/garpix_user/mixins/serializers/to_lower.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.324105 garpix_user-3.8.2/garpix_user/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.8.2/garpix_user/models/access_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/models/refferal.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.8.2/garpix_user/models/refresh_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.8.2/garpix_user/models/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4986 2023-04-24 07:29:27.000000 garpix_user-3.8.2/garpix_user/models/user_session.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.324328 garpix_user-3.8.2/garpix_user/rest/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/rest/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2702 2023-06-23 07:44:40.000000 garpix_user-3.8.2/garpix_user/rest/authentication.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.325492 garpix_user-3.8.2/garpix_user/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      820 2023-06-23 07:44:40.000000 garpix_user-3.8.2/garpix_user/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.8.2/garpix_user/serializers/auth_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/serializers/email_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      247 2023-06-23 07:44:40.000000 garpix_user-3.8.2/garpix_user/serializers/jwt_data_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1584 2023-05-31 09:44:39.000000 garpix_user-3.8.2/garpix_user/serializers/passwrod_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/serializers/phone_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/serializers/refresh_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.8.2/garpix_user/serializers/registration_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.8.2/garpix_user/serializers/user_session_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-07-14 08:27:10.000000 garpix_user-3.8.2/garpix_user/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.325739 garpix_user-3.8.2/garpix_user/tasks/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.8.2/garpix_user/tasks/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.8.2/garpix_user/tasks/delete_unconfirmed_users.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.312117 garpix_user-3.8.2/garpix_user/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.325855 garpix_user-3.8.2/garpix_user/templates/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/templates/garpix_user/send_confirm.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.326256 garpix_user-3.8.2/garpix_user/tests/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/tests/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.326819 garpix_user-3.8.2/garpix_user/tests/test_api/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/tests/test_api/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.327056 garpix_user-3.8.2/garpix_user/tests/test_api/_trial_temp/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/tests/test_api/_trial_temp/_trial_marker
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.8.2/garpix_user/tests/test_api/_trial_temp/test.log
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/tests/test_api/api_login.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/tests/test_api/api_registration.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.8.2/garpix_user/tests/test_api/api_user_session_restore_password.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/tests/test_views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.327407 garpix_user-3.8.2/garpix_user/tests/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/tests/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/tests/utils/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/tests/utils/test_case_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2661 2023-06-21 15:22:29.000000 garpix_user-3.8.2/garpix_user/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.328510 garpix_user-3.8.2/garpix_user/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.8.2/garpix_user/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-06-22 15:00:39.000000 garpix_user-3.8.2/garpix_user/utils/backends.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/utils/current_date.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.8.2/garpix_user/utils/drf_spectacular.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      329 2023-06-23 07:44:40.000000 garpix_user-3.8.2/garpix_user/utils/get_token_from_request.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-07-14 08:19:15.000000 garpix_user-3.8.2/garpix_user/utils/repluralize.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.330144 garpix_user-3.8.2/garpix_user/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/views/change_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.8.2/garpix_user/views/email_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2426 2023-06-23 07:44:40.000000 garpix_user-3.8.2/garpix_user/views/login_views.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.8.2/garpix_user/views/logout_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2942 2023-06-23 07:44:40.000000 garpix_user-3.8.2/garpix_user/views/obtain_auth_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.8.2/garpix_user/views/phone_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/views/referral_links_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.8.2/garpix_user/views/refresh_token_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/views/registration_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3452 2023-05-31 09:44:39.000000 garpix_user-3.8.2/garpix_user/views/restore_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.8.2/garpix_user/views/user_session_view.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-14 08:28:18.320855 garpix_user-3.8.2/garpix_user.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-07-14 08:28:18.000000 garpix_user-3.8.2/garpix_user.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3187 2023-07-14 08:28:18.000000 garpix_user-3.8.2/garpix_user.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-14 08:28:18.000000 garpix_user-3.8.2/garpix_user.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-14 08:28:18.000000 garpix_user-3.8.2/garpix_user.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      279 2023-07-14 08:28:18.000000 garpix_user-3.8.2/garpix_user.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-07-14 08:28:18.000000 garpix_user-3.8.2/garpix_user.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-07-14 08:28:18.330646 garpix_user-3.8.2/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-07-14 08:28:18.000000 garpix_user-3.8.2/setup.py
```

### Comparing `garpix_user-3.8.1/PKG-INFO` & `garpix_user-3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_user
-Version: 3.8.1
+Version: 3.8.2
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.8.1/garpix_user/CHANGELOG.md` & `garpix_user-3.8.2/garpix_user/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 3.8.2 (14.07.2023)
+
+- Error messages localization fixed
+
 ### 3.8.1 (26.06.2023)
 
 - Password restore by username fixed
 
 ### 3.8.0 (22.06.2023)
 
 - JWT token authorization added (see `Readme.md`)
```

### Comparing `garpix_user-3.8.1/garpix_user/CONTRIBUTING.md` & `garpix_user-3.8.2/garpix_user/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/README.md` & `garpix_user-3.8.2/garpix_user/README.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/README.rst` & `garpix_user-3.8.2/garpix_user/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/admin/user.py` & `garpix_user-3.8.2/garpix_user/admin/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/exceptions.py` & `garpix_user-3.8.2/garpix_user/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 from django.conf import settings
 from django.core.validators import ValidationError
 from django.utils.translation import ugettext as _
 from rest_framework import serializers
 
+from garpix_user.utils.repluralize import rupluralize
+
 
 class ModelException(Exception):
-    message = ''
     code = 'invalid'
     field = None
 
     def __init__(self, field=None, extra_data={}):
-        self.message = self.message.format(**extra_data)
+        self.message = self.get_message().format(**extra_data)
         self.field = field
 
     def raise_exception(self, exception_class=ValidationError):
         field = self.field or 'non_field_errors'
         raise exception_class({field: [self.message]}, code=self.code)
 
     def get_message(self):
-        return self.message
+        return ''
 
 
 class WaitException(ModelException):
-    message = settings.GARPIX_USER.get('WAIT_RESPONSE',
-                                       _("Less than {min_time} minutes has passed since the last request")).format(
-        min_time=settings.GARPIX_USER.get('TIME_LAST_REQUEST', 1))
+    def get_message(self):
+        return settings.GARPIX_USER.get('WAIT_RESPONSE',
+                                        _("Less than {min_time} {minutes} has passed since the last request")).format(
+            min_time=settings.GARPIX_USER.get('TIME_LAST_REQUEST', 1),
+            minutes=rupluralize(settings.GARPIX_USER.get('TIME_LAST_REQUEST', 1), _('minute,minutes')))
 
 
 class UserRegisteredException(ModelException):
-    message = settings.GARPIX_USER.get('USER_REGISTERED_RESPONSE',
-                                       _("User with such data has been already registered"))
+    def get_message(self):
+        return settings.GARPIX_USER.get('USER_REGISTERED_RESPONSE',
+                                        _("User with such data has been already registered"))
 
 
 class UserUnregisteredException(ModelException):
-    message = settings.GARPIX_USER.get('USER_UNREGISTERED_RESPONSE', _("User with such data has not been registered"))
+    def get_message(self):
+        return settings.GARPIX_USER.get('USER_UNREGISTERED_RESPONSE', _("User with such data has not been registered"))
 
 
 class IncorrectCodeException(ModelException):
-    message = _("Incorrect code")
+    def get_message(self):
+        return _("Incorrect code")
 
 
 class NoTimeLeftException(ModelException):
-    message = _("Code has expired. Request it again")
+    def get_message(self):
+        return _("Code has expired. Request it again")
 
 
 class NotAuthenticateException(ModelException):
-    message = _("Credentials were not provided")
+    def get_message(self):
+        return _("Credentials were not provided")
 
 
 class NotConfirmedException(ModelException):
-    message = _("{field} was not confirmed")
+    def get_message(self):
+        return _("{field} was not confirmed")
 
 
 class ValidationErrorSerializer(serializers.Serializer):
     field = serializers.ListField(default=['Error'])
```

### Comparing `garpix_user-3.8.1/garpix_user/forms/login.py` & `garpix_user-3.8.2/garpix_user/forms/login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.mo` & `garpix_user-3.8.2/garpix_user/locale/ru/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -60,16 +60,16 @@
 
 msgid "Last entrance"
 msgstr "Последний вход"
 
 msgid "Less than 1 minutes has passed since the last request"
 msgstr "Не прошло 1 минуты с момента последней попытки"
 
-msgid "Less than {min_time} minutes has passed since the last request"
-msgstr "Прошло меньше {min_time} минут с последнего запроса"
+msgid "Less than {min_time} {minutes} has passed since the last request"
+msgstr "Прошло меньше {min_time} {minutes} с последнего запроса"
 
 msgid "New email"
 msgstr "Новый email"
 
 msgid "New phone number"
 msgstr "Новый номер телефона"
 
@@ -154,15 +154,15 @@
 msgid "System users"
 msgstr "Системные пользователи"
 
 msgid "Telegram"
 msgstr "Telegram"
 
 msgid "The phone number entered is not valid."
-msgstr "Введенный некорректный номер телефона."
+msgstr "Введен некорректный номер телефона."
 
 msgid "This email is already in use"
 msgstr "Email уже используется"
 
 msgid "This phone is already in use"
 msgstr "Номер телефона уже используется"
 
@@ -207,14 +207,17 @@
 
 msgid "digit,digits"
 msgstr "цифру,цифры,цифр"
 
 msgid "letter,letters"
 msgstr "заглавную букву,заглавные буквы,заглавных букв"
 
+msgid "minute,minutes"
+msgstr "минуты,минут,минут"
+
 msgid ""
 "{field} can't be used as USERNAME_FIELDS. Only (\"email\", \"phone\", "
 "\"username\") supported"
 msgstr ""
 "{field} не может быть использован в качестве USERNAME_FIELDS. Только "
 "(\"email\", \"phone\", \"username\") поддерживаются"
```

### Comparing `garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.po` & `garpix_user-3.8.2/garpix_user/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -276,25 +276,28 @@
 
 msgid "Restore password. Step 3"
 msgstr "Восстановление пароля. Шаг 3"
 
 msgid "Send email confirmation link"
 msgstr "Отправка ссылки подтверждения email"
 
-msgid "Less than {min_time} minutes has passed since the last request"
-msgstr "Прошло меньше {min_time} минут с последнего запроса"
+msgid "Less than {min_time} {minutes} has passed since the last request"
+msgstr "Прошло меньше {min_time} {minutes} с последнего запроса"
+
+msgid "minute,minutes"
+msgstr "минуты,минут,минут"
 
 msgid "User with such data has been already registered"
 msgstr "Пользователь с указанными данными уже зарегистрирован"
 
 msgid "User with such data has not been registered"
 msgstr "Пользователь с указанными данными не зарегистрирован"
 
 msgid "The phone number entered is not valid."
-msgstr "Введенный некорректный номер телефона."
+msgstr "Введен некорректный номер телефона."
 
 msgid "Password is incorrect"
 msgstr "Некорректный пароль"
 
 msgid "Email or phone number"
 msgstr "Email или номер телефона"
```

### Comparing `garpix_user-3.8.1/garpix_user/mixins/models/confirm/code_length_mixin.py` & `garpix_user-3.8.2/garpix_user/mixins/models/confirm/code_length_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/mixins/models/confirm/email_confirm.py` & `garpix_user-3.8.2/garpix_user/mixins/models/confirm/email_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/mixins/models/confirm/phone_confirm.py` & `garpix_user-3.8.2/garpix_user/mixins/models/confirm/phone_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/mixins/models/restore_password.py` & `garpix_user-3.8.2/garpix_user/mixins/models/restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/mixins/serializers/password_mixin.py` & `garpix_user-3.8.2/garpix_user/mixins/serializers/password_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/models/access_token.py` & `garpix_user-3.8.2/garpix_user/models/access_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/models/refferal.py` & `garpix_user-3.8.2/garpix_user/models/refferal.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/models/refresh_token.py` & `garpix_user-3.8.2/garpix_user/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/models/user.py` & `garpix_user-3.8.2/garpix_user/models/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/models/user_session.py` & `garpix_user-3.8.2/garpix_user/models/user_session.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/rest/authentication.py` & `garpix_user-3.8.2/garpix_user/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/serializers/__init__.py` & `garpix_user-3.8.2/garpix_user/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/serializers/auth_token_serializer.py` & `garpix_user-3.8.2/garpix_user/serializers/auth_token_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/serializers/passwrod_serializer.py` & `garpix_user-3.8.2/garpix_user/serializers/passwrod_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/serializers/registration_serializer.py` & `garpix_user-3.8.2/garpix_user/serializers/registration_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/settings.py` & `garpix_user-3.8.2/garpix_user/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/setup.py` & `garpix_user-3.8.2/garpix_user/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.8.1',
+    version='3.8.2',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_user-3.8.1/garpix_user/tasks/delete_unconfirmed_users.py` & `garpix_user-3.8.2/garpix_user/tasks/delete_unconfirmed_users.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/tests/test_api/api_login.py` & `garpix_user-3.8.2/garpix_user/tests/test_api/api_login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/tests/test_api/api_registration.py` & `garpix_user-3.8.2/garpix_user/tests/test_api/api_registration.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/tests/test_api/api_user_session_restore_password.py` & `garpix_user-3.8.2/garpix_user/tests/test_api/api_user_session_restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/tests/test_views.py` & `garpix_user-3.8.2/garpix_user/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/tests/utils/settings.py` & `garpix_user-3.8.2/garpix_user/tests/utils/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/tests/utils/test_case_mixin.py` & `garpix_user-3.8.2/garpix_user/tests/utils/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/urls.py` & `garpix_user-3.8.2/garpix_user/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/utils/backends.py` & `garpix_user-3.8.2/garpix_user/utils/backends.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/utils/repluralize.py` & `garpix_user-3.8.2/garpix_user/utils/repluralize.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/__init__.py` & `garpix_user-3.8.2/garpix_user/views/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/change_password_view.py` & `garpix_user-3.8.2/garpix_user/views/change_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/email_confirmation_view.py` & `garpix_user-3.8.2/garpix_user/views/email_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/login_views.py` & `garpix_user-3.8.2/garpix_user/views/login_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/logout_view.py` & `garpix_user-3.8.2/garpix_user/views/logout_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/obtain_auth_token.py` & `garpix_user-3.8.2/garpix_user/views/obtain_auth_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/phone_confirmation_view.py` & `garpix_user-3.8.2/garpix_user/views/phone_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/referral_links_view.py` & `garpix_user-3.8.2/garpix_user/views/referral_links_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/refresh_token_view.py` & `garpix_user-3.8.2/garpix_user/views/refresh_token_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/registration_view.py` & `garpix_user-3.8.2/garpix_user/views/registration_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/restore_password_view.py` & `garpix_user-3.8.2/garpix_user/views/restore_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user/views/user_session_view.py` & `garpix_user-3.8.2/garpix_user/views/user_session_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/garpix_user.egg-info/PKG-INFO` & `garpix_user-3.8.2/garpix_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-user
-Version: 3.8.1
+Version: 3.8.2
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.8.1/garpix_user.egg-info/SOURCES.txt` & `garpix_user-3.8.2/garpix_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.1/setup.py` & `garpix_user-3.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.8.1',
+    version='3.8.2',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

