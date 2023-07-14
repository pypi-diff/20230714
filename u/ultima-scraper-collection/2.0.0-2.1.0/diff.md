# Comparing `tmp/ultima_scraper_collection-2.0.0.tar.gz` & `tmp/ultima_scraper_collection-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-2.0.0.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-2.1.0.tar", max compression
```

## Comparing `ultima_scraper_collection-2.0.0.tar` & `ultima_scraper_collection-2.1.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      881 2023-07-12 18:52:02.405662 ultima_scraper_collection-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-2.0.0/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0     3547 2023-07-13 05:55:18.678148 ultima_scraper_collection-2.0.0/ultima_scraper_collection/config.py
--rw-r--r--   0        0        0        0 2023-07-12 11:29:22.237223 ultima_scraper_collection-2.0.0/ultima_scraper_collection/helpers/__init__.py
--rw-r--r--   0        0        0     1216 2023-07-12 09:07:53.912599 ultima_scraper_collection-2.0.0/ultima_scraper_collection/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-03 17:34:00.273754 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0     9956 2023-06-15 07:56:54.052868 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     2293 2023-07-12 11:08:07.047292 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0     5349 2023-07-13 02:40:41.499162 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0     5637 2023-07-13 02:40:59.485296 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0    11385 2023-07-12 12:04:54.350746 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    17461 2023-07-13 06:10:56.309738 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0    29639 2023-07-13 06:00:04.516010 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     7127 2023-07-13 05:58:14.304809 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0     5769 2023-07-13 05:58:45.954199 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/server_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-2.0.0/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    16177 2023-07-13 05:54:18.325942 ultima_scraper_collection-2.0.0/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-2.0.0/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 ultima_scraper_collection-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      881 2023-07-14 08:54:08.149193 ultima_scraper_collection-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-2.1.0/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0     3547 2023-07-13 05:55:18.678148 ultima_scraper_collection-2.1.0/ultima_scraper_collection/config.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:29:22.237223 ultima_scraper_collection-2.1.0/ultima_scraper_collection/helpers/__init__.py
+-rw-r--r--   0        0        0     2312 2023-07-14 07:33:04.022710 ultima_scraper_collection-2.1.0/ultima_scraper_collection/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-03 17:34:00.273754 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0     9956 2023-06-15 07:56:54.052868 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     2293 2023-07-12 11:08:07.047292 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0     5349 2023-07-13 02:40:41.499162 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     5637 2023-07-13 02:40:59.485296 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0    11385 2023-07-12 12:04:54.350746 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    17461 2023-07-13 06:10:56.309738 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    29632 2023-07-14 06:01:01.875819 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     7127 2023-07-13 05:58:14.304809 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0     6049 2023-07-13 18:11:24.830592 ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/server_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-2.1.0/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    16231 2023-07-13 21:04:13.077641 ultima_scraper_collection-2.1.0/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-2.1.0/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 ultima_scraper_collection-2.1.0/PKG-INFO
```

### Comparing `ultima_scraper_collection-2.0.0/pyproject.toml` & `ultima_scraper_collection-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "2.0.0"
+version = "2.1.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_collection"}]
 include = ["ultima_scraper_collection/py.typed"]
```

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/config.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/config.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/download_manager.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/download_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 from pathlib import Path
 from typing import Any, TypedDict
 from urllib.parse import ParseResult, urlparse
 
 import ultima_scraper_api
 from sqlalchemy import inspect
 from ultima_scraper_api.helpers import main_helper
+from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
+    DBCollection,
+    SqliteDatabase,
+)
+from ultima_scraper_collection.managers.database_manager.database_manager import (
+    DatabaseManager,
+)
+from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_db.databases.ultima.schemas.templates.site import (
     MediaModel as DBMediaModel,
 )
 from ultima_scraper_db.databases.ultima.schemas.templates.site import (
     MessageModel as DBMessageModel,
 )
 from ultima_scraper_db.databases.ultima.schemas.templates.site import (
     PostModel as DBPostModel,
 )
 from ultima_scraper_db.databases.ultima.schemas.templates.site import (
     StoryModel as DBStoryModel,
 )
 
-from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
-    DBCollection,
-    SqliteDatabase,
-)
-from ultima_scraper_collection.managers.database_manager.database_manager import (
-    DatabaseManager,
-)
-from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
-
 api_types = ultima_scraper_api.api_types
 user_types = ultima_scraper_api.user_types
 content_types = ultima_scraper_api.content_types
 
 
 class DBContentExtractor:
     def __init__(
@@ -145,15 +144,15 @@
         temp_date = self.item.created_at
         assert temp_date
         if isinstance(temp_date, str):
             try:
                 temp_date = float(temp_date)
             except:
                 pass
-        default_date = datetime.utcnow()
+        default_date = datetime.now()
         if temp_date == "-001-11-30T00:00:00+00:00":
             date_object = default_date
         else:
             if not temp_date:
                 temp_date = default_date
             if isinstance(temp_date, int):
                 timestamp = float(temp_date)
@@ -219,15 +218,15 @@
     def resolve_archived(self):
         archived = False
         if isinstance(self.item, ultima_scraper_api.post_types):
             archived = self.item.isArchived
         return archived
 
     def resolve_paid(self):
-        if getattr(self.item, "price", 0):
+        if hasattr(self.item, "price"):
             if all(media["canView"] for media in self.item.media):
                 return True
             return False
         else:
             return None
 
     def get_receiver_id(self):
@@ -256,19 +255,19 @@
     async def resolve_extractor(self, result: ApiExtractor | DBContentExtractor):
         self.content_id = result.get_id()
         self.user_id = result.get_user_id()
         self.receiver_id = result.get_receiver_id()
         self.text = result.get_text()
         self.preview_media_ids = result.get_preview_ids()
         self.archived = result.resolve_archived()
-        self.medias: list[MediaMetadata] = await result.get_medias(self)
         self.price = getattr(result.item, "price", 0) or 0
         self.paid = result.resolve_paid()
         self.deleted = False
         self.created_at: datetime = result.get_date()
+        self.medias: list[MediaMetadata] = await result.get_medias(self)
         self.__raw__: Any | None = None
         self.__soft__ = result.item
         self.__media_types__ = None
 
     def find_media(self, media_id: int | None = None, urls: list[str] = []):
         for asset in self.medias:
             if asset.id == media_id:
```

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/option_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/server_manager.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/managers/server_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import netifaces
 import paramiko
 
 # from degen_x.managers.database_manager.database_manager import DatabaseManager
 # from degen_x.managers.database_manager.job_manager import JobManager
 # from degen_x.managers.database_manager.legacy import legacy_to_new
 from sqlalchemy import MetaData, select
-from sshtunnel import SSHTunnelForwarder#type: ignore
+from sshtunnel import SSHTunnelForwarder  # type: ignore
 from ultima_scraper_db.databases.ultima.schemas.management import ServerModel, SiteModel
 from ultima_scraper_db.managers.database_manager import Alembica, DatabaseManager
+from ultima_scraper_db.managers.database_manager import Schema
 
 if TYPE_CHECKING:
     from ultima_scraper_collection import datascraper_types
 
 
 class ServerManager:
     def __init__(
@@ -114,14 +115,18 @@
         active_server = await self.management_db.session.scalars(
             select(ServerModel).where(
                 (ServerModel.ip == self.ip_address)
                 & (ServerModel.mac_address == mac_address)
             )
         )
         self.active_server = active_server.one()
+        self.site_schemas: list[Schema] = []
+        for db_site in self.db_sites:
+            site_schema_api = await self.get_site_db(db_site.db_name)
+            self.site_schemas.append(site_schema_api.schema)
         return self
 
     async def get_site_db(
         self, name: str, datascraper: "datascraper_types | None" = None
     ):
         from ultima_scraper_db.managers.site_db import SiteDB
```

### Comparing `ultima_scraper_collection-2.0.0/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-2.1.0/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 import copy
 from itertools import product
 from typing import Any, Optional
 
 import ultima_scraper_api
 from sqlalchemy import and_, or_, select
 from tqdm.asyncio import tqdm_asyncio
-from ultima_scraper_db.databases.ultima.schemas.templates.site import (
-    MessageModel as DBMessageModel,
-)
-
 from ultima_scraper_collection.config import site_config_types
 from ultima_scraper_collection.managers.download_manager import DownloadManager
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     MetadataManager,
 )
 from ultima_scraper_collection.managers.server_manager import ServerManager
+from ultima_scraper_db.databases.ultima.schemas.templates.site import (
+    MessageModel as DBMessageModel,
+)
 
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
 message_types = ultima_scraper_api.message_types
 error_types = ultima_scraper_api.error_types
 subscription_types = ultima_scraper_api.subscription_types
 from typing import TYPE_CHECKING
@@ -277,15 +276,16 @@
             return
         api = performer.get_api()
         assert current_job
         site_db = await self.server_manager.get_site_db(api.site_name, self.datascraper)
         db_user = await site_db.get_user(performer.id)
         assert db_user
         await db_user.awaitable_attrs.content_manager
-        db_contents = await db_user.content_manager.get_contents(api_type)
+        content_manager = await db_user.content_manager.init()
+        db_contents = await content_manager.get_contents(api_type)
         final_download_set: set[ContentMetadata] = set()
         total_media_count = 0
         download_media_count = 0
         for db_content in db_contents:
             await site_db.session.refresh(db_content, ["media"])
             # To find duplicates, we must check if media belongs to any other content type via association table
             found_content = performer.content_manager.find_content(
```

### Comparing `ultima_scraper_collection-2.0.0/PKG-INFO` & `ultima_scraper_collection-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 2.0.0
+Version: 2.1.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

