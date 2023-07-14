# Comparing `tmp/lspace-0.4.5.tar.gz` & `tmp/lspace-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lspace-0.4.5.tar", last modified: Sun Aug 28 11:39:07 2022, max compression
+gzip compressed data, was "lspace-0.4.6.tar", last modified: Fri Jul 14 14:28:49 2023, max compression
```

## Comparing `lspace-0.4.5.tar` & `lspace-0.4.6.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.023963 lspace-0.4.5/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)    34523 2019-06-29 12:44:12.000000 lspace-0.4.5/LICENSE
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      257 2022-08-28 11:23:26.000000 lspace-0.4.5/MANIFEST.in
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     6443 2022-08-28 11:39:07.023963 lspace-0.4.5/PKG-INFO
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     5622 2022-08-28 11:28:31.000000 lspace-0.4.5/README.md
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.000630 lspace-0.4.5/lspace/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2787 2022-08-28 11:36:10.000000 lspace-0.4.5/lspace/__init__.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.003964 lspace-0.4.5/lspace/api_v1_blueprint/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      701 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/api_v1_blueprint/__init__.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.003964 lspace-0.4.5/lspace/api_v1_blueprint/models/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2374 2020-02-23 18:51:53.000000 lspace-0.4.5/lspace/api_v1_blueprint/models/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1606 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/api_v1_blueprint/resource_helpers.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.003964 lspace-0.4.5/lspace/api_v1_blueprint/resources/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/api_v1_blueprint/resources/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1659 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/api_v1_blueprint/resources/book.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      689 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/api_v1_blueprint/resources/book_file.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      195 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/api_v1_blueprint/resources/version.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      316 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/app.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.007297 lspace-0.4.5/lspace/cli/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      458 2022-02-18 00:17:50.000000 lspace-0.4.5/lspace/cli/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      273 2019-05-19 23:44:32.000000 lspace-0.4.5/lspace/cli/db_command.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2536 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/cli/export_command.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.007297 lspace-0.4.5/lspace/cli/import_command/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      752 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/cli/import_command/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     8045 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/cli/import_command/_import.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      663 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/cli/import_command/add_book_to_db.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1646 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/cli/import_command/add_to_shelf.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.010630 lspace-0.4.5/lspace/cli/import_command/add_to_shelf_options/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/cli/import_command/add_to_shelf_options/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      295 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/cli/import_command/add_to_shelf_options/_options.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      326 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/cli/import_command/add_to_shelf_options/put_in_default_shelf.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      828 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/cli/import_command/add_to_shelf_options/put_in_new_shelf.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      263 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/base_helper.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      741 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/check_if_in_library.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2834 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/cli/import_command/copy_to_library.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.010630 lspace-0.4.5/lspace/cli/import_command/import_from_api/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3269 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/cli/import_command/import_from_api/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3974 2019-06-21 13:01:41.000000 lspace-0.4.5/lspace/cli/import_command/import_from_calibre.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.010630 lspace-0.4.5/lspace/cli/import_command/import_options/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/import_options/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      548 2019-12-20 12:44:43.000000 lspace-0.4.5/lspace/cli/import_command/import_options/_options.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      457 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/import_options/isbn_lookup.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2956 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/import_options/manual_import.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      359 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/import_options/manual_search.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      312 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/import_options/peek.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      205 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/import_command/import_options/skip_book.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      703 2019-06-03 19:00:30.000000 lspace-0.4.5/lspace/cli/init_command.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1128 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/cli/list_command.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      959 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/reimport_command.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1169 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/cli/remove_command.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.013963 lspace-0.4.5/lspace/cli/tools_command/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1122 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/cli/tools_command/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      343 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/cli/tools_command/clear_cache.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      243 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/cli/tools_command/rebuild_search_index.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1271 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/cli/tools_command/update_paths.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      156 2019-05-22 19:26:59.000000 lspace-0.4.5/lspace/cli/version_command.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1495 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/cli/web_command.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.013963 lspace-0.4.5/lspace/file_types/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      402 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/file_types/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3763 2019-12-20 12:44:43.000000 lspace-0.4.5/lspace/file_types/_base.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1388 2020-04-03 19:39:57.000000 lspace-0.4.5/lspace/file_types/epub.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1744 2019-06-04 20:40:25.000000 lspace-0.4.5/lspace/file_types/pdf.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.013963 lspace-0.4.5/lspace/frontend_blueprint/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1724 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/frontend_blueprint/__init__.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.013963 lspace-0.4.5/lspace/frontend_blueprint/static/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)   190593 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/frontend_blueprint/static/bulma.min.css
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      260 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/frontend_blueprint/static/style.css
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.013963 lspace-0.4.5/lspace/frontend_blueprint/templates/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2525 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/frontend_blueprint/templates/base.html.jinja2
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      610 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/frontend_blueprint/templates/books.html.jinja2
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     4329 2019-08-15 15:13:13.000000 lspace-0.4.5/lspace/frontend_blueprint/templates/macros.html.jinja2
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.017297 lspace-0.4.5/lspace/helpers/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1382 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/helpers/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1016 2019-06-11 22:56:47.000000 lspace-0.4.5/lspace/helpers/init_logging.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2798 2022-02-18 11:39:26.000000 lspace-0.4.5/lspace/helpers/query.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.017297 lspace-0.4.5/lspace/migrations/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       38 2019-05-11 12:42:29.000000 lspace-0.4.5/lspace/migrations/README
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      267 2019-06-11 22:56:47.000000 lspace-0.4.5/lspace/migrations/alembic.ini
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2833 2019-06-11 22:56:47.000000 lspace-0.4.5/lspace/migrations/env.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      494 2019-05-11 12:42:29.000000 lspace-0.4.5/lspace/migrations/script.py.mako
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.017297 lspace-0.4.5/lspace/migrations/versions/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      676 2019-06-14 08:37:11.000000 lspace-0.4.5/lspace/migrations/versions/91732d5540b9_.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1630 2019-06-14 08:37:11.000000 lspace-0.4.5/lspace/migrations/versions/b142d6d9e8da_.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1234 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/migrations/versions/b9f9b5b4e882_.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      804 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/migrations/versions/d8f2fb9f2472_.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      917 2019-06-14 08:37:11.000000 lspace-0.4.5/lspace/migrations/versions/e2bbe7fd9bc7_.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.020630 lspace-0.4.5/lspace/models/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      143 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/models/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      666 2020-02-23 10:32:12.000000 lspace-0.4.5/lspace/models/author.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     5047 2022-07-19 22:35:26.000000 lspace-0.4.5/lspace/models/book.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      598 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/models/book_author_association.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      702 2019-06-16 13:31:16.000000 lspace-0.4.5/lspace/models/meta_cache.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      364 2019-06-29 12:44:12.000000 lspace-0.4.5/lspace/models/shelf.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.003964 lspace-0.4.5/lspace.egg-info/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     6443 2022-08-28 11:39:06.000000 lspace-0.4.5/lspace.egg-info/PKG-INFO
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3432 2022-08-28 11:39:06.000000 lspace-0.4.5/lspace.egg-info/SOURCES.txt
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        1 2022-08-28 11:39:06.000000 lspace-0.4.5/lspace.egg-info/dependency_links.txt
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       67 2022-08-28 11:39:06.000000 lspace-0.4.5/lspace.egg-info/entry_points.txt
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      925 2022-08-28 11:39:06.000000 lspace-0.4.5/lspace.egg-info/requires.txt
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       13 2022-08-28 11:39:06.000000 lspace-0.4.5/lspace.egg-info/top_level.txt
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       38 2022-08-28 11:39:07.023963 lspace-0.4.5/setup.cfg
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2427 2022-08-28 11:36:10.000000 lspace-0.4.5/setup.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.020630 lspace-0.4.5/tests/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-05-19 23:44:32.000000 lspace-0.4.5/tests/__init__.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.020630 lspace-0.4.5/tests/cli/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-05-22 19:26:59.000000 lspace-0.4.5/tests/cli/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1544 2019-06-12 19:58:39.000000 lspace-0.4.5/tests/cli/_cli_test_base.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.020630 lspace-0.4.5/tests/cli/import_command/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-11 21:42:51.000000 lspace-0.4.5/tests/cli/import_command/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1930 2019-06-21 13:01:41.000000 lspace-0.4.5/tests/cli/import_command/test_calibre_meta_file.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1719 2019-06-16 13:31:16.000000 lspace-0.4.5/tests/cli/import_command/test_copy_to_library.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      427 2019-06-11 21:42:51.000000 lspace-0.4.5/tests/cli/test_init_command.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1144 2019-06-11 21:42:51.000000 lspace-0.4.5/tests/cli/test_list_command.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      423 2019-06-11 21:42:51.000000 lspace-0.4.5/tests/cli/test_remove_command.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.020630 lspace-0.4.5/tests/cli/tools/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-11 21:42:51.000000 lspace-0.4.5/tests/cli/tools/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1297 2019-06-16 13:31:16.000000 lspace-0.4.5/tests/cli/tools/test_update_paths.py
-drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2022-08-28 11:39:07.020630 lspace-0.4.5/tests/file_types/
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-16 13:31:16.000000 lspace-0.4.5/tests/file_types/__init__.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2551 2019-06-16 13:31:16.000000 lspace-0.4.5/tests/file_types/test_base.py
--rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      348 2019-05-19 23:44:32.000000 lspace-0.4.5/tests/test_create_app.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.527501 lspace-0.4.6/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)    34523 2019-06-29 12:44:12.000000 lspace-0.4.6/LICENSE
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      217 2022-08-28 12:25:21.000000 lspace-0.4.6/MANIFEST.in
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     6304 2023-07-14 14:28:49.524168 lspace-0.4.6/PKG-INFO
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     5622 2023-07-14 14:24:51.000000 lspace-0.4.6/README.md
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.507502 lspace-0.4.6/lspace/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      938 2023-07-14 14:25:40.000000 lspace-0.4.6/lspace/__init__.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.510835 lspace-0.4.6/lspace/api_v1_blueprint/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      701 2022-02-18 11:39:26.000000 lspace-0.4.6/lspace/api_v1_blueprint/__init__.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.510835 lspace-0.4.6/lspace/api_v1_blueprint/models/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2374 2020-02-23 18:51:53.000000 lspace-0.4.6/lspace/api_v1_blueprint/models/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1606 2022-02-18 11:39:26.000000 lspace-0.4.6/lspace/api_v1_blueprint/resource_helpers.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.510835 lspace-0.4.6/lspace/api_v1_blueprint/resources/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/api_v1_blueprint/resources/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1659 2022-02-18 11:39:26.000000 lspace-0.4.6/lspace/api_v1_blueprint/resources/book.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      671 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/api_v1_blueprint/resources/book_file.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      195 2022-02-18 11:39:26.000000 lspace-0.4.6/lspace/api_v1_blueprint/resources/version.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.510835 lspace-0.4.6/lspace/cli/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      517 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      283 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/db_command.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2546 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/export_command.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.514168 lspace-0.4.6/lspace/cli/import_command/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      762 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/import_command/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     8045 2022-07-19 22:35:26.000000 lspace-0.4.6/lspace/cli/import_command/_import.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      663 2022-07-19 22:35:26.000000 lspace-0.4.6/lspace/cli/import_command/add_book_to_db.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1646 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/cli/import_command/add_to_shelf.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.514168 lspace-0.4.6/lspace/cli/import_command/add_to_shelf_options/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/cli/import_command/add_to_shelf_options/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      295 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/cli/import_command/add_to_shelf_options/_options.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      326 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/cli/import_command/add_to_shelf_options/put_in_default_shelf.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      828 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/cli/import_command/add_to_shelf_options/put_in_new_shelf.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      263 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/base_helper.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      741 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/check_if_in_library.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2834 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/cli/import_command/copy_to_library.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.514168 lspace-0.4.6/lspace/cli/import_command/import_from_api/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3269 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/cli/import_command/import_from_api/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3974 2019-06-21 13:01:41.000000 lspace-0.4.6/lspace/cli/import_command/import_from_calibre.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.517501 lspace-0.4.6/lspace/cli/import_command/import_options/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/import_options/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      548 2019-12-20 12:44:43.000000 lspace-0.4.6/lspace/cli/import_command/import_options/_options.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      457 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/import_options/isbn_lookup.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2956 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/import_options/manual_import.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      359 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/import_options/manual_search.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      312 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/import_options/peek.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      205 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/import_command/import_options/skip_book.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      713 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/init_command.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1138 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/list_command.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      969 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/reimport_command.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1179 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/remove_command.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.517501 lspace-0.4.6/lspace/cli/tools_command/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1132 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/tools_command/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      343 2022-02-18 11:39:26.000000 lspace-0.4.6/lspace/cli/tools_command/clear_cache.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      243 2022-02-18 11:39:26.000000 lspace-0.4.6/lspace/cli/tools_command/rebuild_search_index.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1271 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/cli/tools_command/update_paths.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      166 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/version_command.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1580 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/cli/web_command.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.517501 lspace-0.4.6/lspace/file_types/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      402 2022-07-19 22:35:26.000000 lspace-0.4.6/lspace/file_types/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3763 2019-12-20 12:44:43.000000 lspace-0.4.6/lspace/file_types/_base.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1520 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/file_types/epub.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1727 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/file_types/pdf.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.517501 lspace-0.4.6/lspace/frontend_blueprint/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1724 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/frontend_blueprint/__init__.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.517501 lspace-0.4.6/lspace/frontend_blueprint/static/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)   190593 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/frontend_blueprint/static/bulma.min.css
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      260 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/frontend_blueprint/static/style.css
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.520835 lspace-0.4.6/lspace/frontend_blueprint/templates/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2525 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/frontend_blueprint/templates/base.html.jinja2
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      610 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/frontend_blueprint/templates/books.html.jinja2
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     4329 2019-08-15 15:13:13.000000 lspace-0.4.6/lspace/frontend_blueprint/templates/macros.html.jinja2
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.520835 lspace-0.4.6/lspace/helpers/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1382 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/helpers/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2329 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/helpers/create_app.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1016 2019-06-11 22:56:47.000000 lspace-0.4.6/lspace/helpers/init_logging.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2821 2023-07-14 14:24:51.000000 lspace-0.4.6/lspace/helpers/query.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.520835 lspace-0.4.6/lspace/migrations/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       38 2019-05-11 12:42:29.000000 lspace-0.4.6/lspace/migrations/README
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      267 2019-06-11 22:56:47.000000 lspace-0.4.6/lspace/migrations/alembic.ini
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2833 2019-06-11 22:56:47.000000 lspace-0.4.6/lspace/migrations/env.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      494 2019-05-11 12:42:29.000000 lspace-0.4.6/lspace/migrations/script.py.mako
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.520835 lspace-0.4.6/lspace/migrations/versions/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      676 2019-06-14 08:37:11.000000 lspace-0.4.6/lspace/migrations/versions/91732d5540b9_.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1630 2019-06-14 08:37:11.000000 lspace-0.4.6/lspace/migrations/versions/b142d6d9e8da_.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1234 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/migrations/versions/b9f9b5b4e882_.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      804 2022-07-19 22:35:26.000000 lspace-0.4.6/lspace/migrations/versions/d8f2fb9f2472_.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      917 2019-06-14 08:37:11.000000 lspace-0.4.6/lspace/migrations/versions/e2bbe7fd9bc7_.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.524168 lspace-0.4.6/lspace/models/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      143 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/models/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      666 2023-07-14 10:31:40.000000 lspace-0.4.6/lspace/models/author.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     5047 2023-07-14 10:31:40.000000 lspace-0.4.6/lspace/models/book.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      598 2023-07-14 10:31:47.000000 lspace-0.4.6/lspace/models/book_author_association.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      702 2019-06-16 13:31:16.000000 lspace-0.4.6/lspace/models/meta_cache.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      364 2019-06-29 12:44:12.000000 lspace-0.4.6/lspace/models/shelf.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.507502 lspace-0.4.6/lspace.egg-info/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     6304 2023-07-14 14:28:49.000000 lspace-0.4.6/lspace.egg-info/PKG-INFO
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     3447 2023-07-14 14:28:49.000000 lspace-0.4.6/lspace.egg-info/SOURCES.txt
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        1 2023-07-14 14:28:49.000000 lspace-0.4.6/lspace.egg-info/dependency_links.txt
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       38 2023-07-14 14:28:49.000000 lspace-0.4.6/lspace.egg-info/entry_points.txt
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      959 2023-07-14 14:28:49.000000 lspace-0.4.6/lspace.egg-info/requires.txt
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       13 2023-07-14 14:28:49.000000 lspace-0.4.6/lspace.egg-info/top_level.txt
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)       38 2023-07-14 14:28:49.527501 lspace-0.4.6/setup.cfg
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2381 2023-07-14 14:25:40.000000 lspace-0.4.6/setup.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.524168 lspace-0.4.6/tests/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-05-19 23:44:32.000000 lspace-0.4.6/tests/__init__.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.524168 lspace-0.4.6/tests/cli/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-05-22 19:26:59.000000 lspace-0.4.6/tests/cli/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1544 2019-06-12 19:58:39.000000 lspace-0.4.6/tests/cli/_cli_test_base.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.524168 lspace-0.4.6/tests/cli/import_command/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-11 21:42:51.000000 lspace-0.4.6/tests/cli/import_command/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1930 2019-06-21 13:01:41.000000 lspace-0.4.6/tests/cli/import_command/test_calibre_meta_file.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1719 2019-06-16 13:31:16.000000 lspace-0.4.6/tests/cli/import_command/test_copy_to_library.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      427 2019-06-11 21:42:51.000000 lspace-0.4.6/tests/cli/test_init_command.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1144 2019-06-11 21:42:51.000000 lspace-0.4.6/tests/cli/test_list_command.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      423 2019-06-11 21:42:51.000000 lspace-0.4.6/tests/cli/test_remove_command.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.524168 lspace-0.4.6/tests/cli/tools/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-11 21:42:51.000000 lspace-0.4.6/tests/cli/tools/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     1297 2019-06-16 13:31:16.000000 lspace-0.4.6/tests/cli/tools/test_update_paths.py
+drwxr-xr-x   0 meatpuppet  (1000) meatpuppet  (1000)        0 2023-07-14 14:28:49.524168 lspace-0.4.6/tests/file_types/
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)        0 2019-06-16 13:31:16.000000 lspace-0.4.6/tests/file_types/__init__.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)     2551 2019-06-16 13:31:16.000000 lspace-0.4.6/tests/file_types/test_base.py
+-rw-r--r--   0 meatpuppet  (1000) meatpuppet  (1000)      348 2019-05-19 23:44:32.000000 lspace-0.4.6/tests/test_create_app.py
```

### Comparing `lspace-0.4.5/LICENSE` & `lspace-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/PKG-INFO` & `lspace-0.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: lspace
-Version: 0.4.5
-Summary: a ebook manager built around isbnlib
+Version: 0.4.6
+Summary: ebook manager built around isbnlib
 Home-page: https://github.com/puhoy/lspace
 Author: jan
 Author-email: stuff@kwoh.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
-# L-Space
+# l-space
 
 a cli ebook manager built around [isbnlib](https://github.com/xlcnd/isbnlib)
 
-when importing it tries to find isbns in the files metadata and in the text. 
+on import, lspace tries to find isbns in the files metadata and in the text. 
 with the isbn it tries to fetch metadata about the book from google books and openlibrary. 
 if no isbn is found, it queries metadata based on the filename.
 
 after this, your properly renamed files will be stored in your library folder.
 
 currently supports epub and pdf.
 
@@ -235,9 +231,7 @@
 bumping is requires bump2version, twine is used for uploading to pypi.
 
 
 ## why "L-space"?
 
 its named after discworlds [library-space](https://en.wikipedia.org/wiki/List_of_dimensions_of_the_Discworld#L-space) dimension :)
 
-
-
```

### Comparing `lspace-0.4.5/README.md` & `lspace-0.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# L-Space
+# l-space
 
 a cli ebook manager built around [isbnlib](https://github.com/xlcnd/isbnlib)
 
-when importing it tries to find isbns in the files metadata and in the text. 
+on import, lspace tries to find isbns in the files metadata and in the text. 
 with the isbn it tries to fetch metadata about the book from google books and openlibrary. 
 if no isbn is found, it queries metadata based on the filename.
 
 after this, your properly renamed files will be stored in your library folder.
 
 currently supports epub and pdf.
```

### Comparing `lspace-0.4.5/lspace/api_v1_blueprint/__init__.py` & `lspace-0.4.6/lspace/api_v1_blueprint/__init__.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/api_v1_blueprint/models/__init__.py` & `lspace-0.4.6/lspace/api_v1_blueprint/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/api_v1_blueprint/resource_helpers.py` & `lspace-0.4.6/lspace/api_v1_blueprint/resource_helpers.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/api_v1_blueprint/resources/book.py` & `lspace-0.4.6/lspace/api_v1_blueprint/resources/book.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/export_command.py` & `lspace-0.4.6/lspace/cli/export_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import shutil
 import subprocess
 
 import click
 from slugify import slugify
 
 from flask import current_app
-from lspace.cli import cli
+from lspace.cli import cli_bp
 from lspace.cli.import_command.copy_to_library import find_unused_path
 from lspace.helpers.query import query_db
 
 logger = logging.getLogger(__name__)
 
 
-@cli.command(help='export books to a folder - this uses ebook-convert, which is part of calibre')
+@cli_bp.cli.command(help='export books to a folder - this uses ebook-convert, which is part of calibre')
 @click.argument('query', nargs=-1)
 @click.argument('export_path')
 @click.option('--format')
 def export(query, export_path, format):
     if format:
         if not shutil.which('ebook-convert'):
             click.echo('could not find ebook-convert executable! is calibre installed?')
```

### Comparing `lspace-0.4.5/lspace/cli/import_command/__init__.py` & `lspace-0.4.6/lspace/cli/import_command/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 
-from lspace.cli import cli
+from lspace.cli import cli_bp
 from lspace.cli.import_command._import import import_wizard
 
 
-@cli.command(name='import', help='import ebooks into your database')
+@cli_bp.cli.command(name='import', help='import ebooks into your database')
 @click.argument('document_path', type=click.Path(), nargs=-1)
 @click.option('--skip-library-check', help='dont check if this file is in the library already', default=False,
               is_flag=True)
 @click.option('--move', help='move imported files instead copying', default=False, is_flag=True)
 @click.option('--inplace', help='add this file to the library, but keep it where it is', default=False, is_flag=True)
 def import_command(document_path, skip_library_check, move, inplace):
     for path in document_path:
```

### Comparing `lspace-0.4.5/lspace/cli/import_command/_import.py` & `lspace-0.4.6/lspace/cli/import_command/_import.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/add_book_to_db.py` & `lspace-0.4.6/lspace/cli/import_command/add_book_to_db.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/add_to_shelf.py` & `lspace-0.4.6/lspace/cli/import_command/add_to_shelf.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/add_to_shelf_options/put_in_new_shelf.py` & `lspace-0.4.6/lspace/cli/import_command/add_to_shelf_options/put_in_new_shelf.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/check_if_in_library.py` & `lspace-0.4.6/lspace/cli/import_command/check_if_in_library.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/copy_to_library.py` & `lspace-0.4.6/lspace/cli/import_command/copy_to_library.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/import_from_api/__init__.py` & `lspace-0.4.6/lspace/cli/import_command/import_from_api/__init__.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/import_from_calibre.py` & `lspace-0.4.6/lspace/cli/import_command/import_from_calibre.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/import_options/_options.py` & `lspace-0.4.6/lspace/cli/import_command/import_options/_options.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/import_command/import_options/manual_import.py` & `lspace-0.4.6/lspace/cli/import_command/import_options/manual_import.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/init_command.py` & `lspace-0.4.6/lspace/cli/init_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 import click
 import yaml
 
 from lspace.helpers import get_default_config
-from lspace.cli import cli
+from lspace.cli import cli_bp
 
 
-@cli.command(help='generate a new config')
+@cli_bp.cli.command(help='generate a new config')
 def init():
     from flask import current_app
 
     app_dir = current_app.config['APP_DIR']
     config_path = current_app.config['CONFIG_PATH']
 
     if not os.path.isdir(app_dir):
```

### Comparing `lspace-0.4.5/lspace/cli/list_command.py` & `lspace-0.4.6/lspace/cli/list_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 
-from lspace.cli import cli
+from lspace.cli import cli_bp
 from lspace.helpers.query import query_db
 
 
-@cli.command(name='list', help='query your database')
+@cli_bp.cli.command(name='list', help='query your database')
 @click.argument('query', nargs=-1)
 @click.option('--path', is_flag=True)
 @click.option('--details', is_flag=True)
 def _list(query, path, details):
     results = query_db(query)
 
     if path:
```

### Comparing `lspace-0.4.5/lspace/cli/reimport_command.py` & `lspace-0.4.6/lspace/cli/reimport_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import click
 
 from lspace.cli.import_command import import_wizard
-from lspace.cli import cli
+from lspace.cli import cli_bp
 from lspace import db
 from lspace.helpers.query import query_db
 
 
-@cli.command(help='reimport books in library')
+@cli_bp.cli.command(help='reimport books in library')
 @click.argument('query', nargs=-1)
 def reimport(query):
     if not query:
         exit()
     results = query_db(query)
     
     for result in results:
```

### Comparing `lspace-0.4.5/lspace/cli/remove_command.py` & `lspace-0.4.6/lspace/cli/remove_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import click
 
-from lspace.cli import cli
+from lspace.cli import cli_bp
 from lspace.helpers.query import query_db
 from lspace import db
 
 
-@cli.command(help='remove books from library')
+@cli_bp.cli.command(help='remove books from library')
 @click.argument('query', nargs=-1)
 def remove(query):
     if not query:
         exit()
     results = query_db(query)
     
     for result in results:
```

### Comparing `lspace-0.4.5/lspace/cli/tools_command/__init__.py` & `lspace-0.4.6/lspace/cli/tools_command/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
 import click
 import isbnlib
 import yaml
 
-from lspace.cli import cli
+from lspace.cli import cli_bp
 
 logger = logging.getLogger(__name__)
 
 
-@cli.group(help='tools you probably never need... :P')
+@cli_bp.cli.group(help='tools you probably never need... :P')
 def tools():
     pass
 
 
 from lspace.cli.tools_command.clear_cache import clear_cache
 from lspace.cli.tools_command.rebuild_search_index import rebuild_search_index
 from lspace.cli.tools_command.update_paths import _update_paths
```

### Comparing `lspace-0.4.5/lspace/cli/tools_command/update_paths.py` & `lspace-0.4.6/lspace/cli/tools_command/update_paths.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/cli/web_command.py` & `lspace-0.4.6/lspace/cli/web_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import os
 
+
 import click
 import gunicorn.app.base
+from flask import current_app
 
 from lspace.api_v1_blueprint import api_blueprint
-from lspace.app import app
-from lspace.cli import cli
+from lspace.cli import cli_bp
 from lspace.frontend_blueprint import frontend_blueprint
 
 
-@cli.command(help='start a webserver')
+@cli_bp.cli.command(help='start a webserver')
 @click.option('--port', default=5000)
 @click.option('--host', default='0.0.0.0')
 @click.option('--debug', default=False, is_flag=True)
 def web(host, port, debug):
-    app.register_blueprint(api_blueprint, url_prefix='/api/v1')
-    app.register_blueprint(frontend_blueprint, url_prefix='')
+    current_app.register_blueprint(api_blueprint, url_prefix='/api/v1')
+    current_app.register_blueprint(frontend_blueprint, url_prefix='')
 
+    # todo: flask_env removed in 2.3.0
     if (os.environ.get('LSPACE_DEV', None) == '1') or debug:
         os.environ['FLASK_ENV'] = 'development'
         print(os.environ['FLASK_ENV'])
-        app.run(debug=True, host=host, port=port)
+        current_app.run(debug=True, host=host, port=port)
     else:
         options = {
             'bind': '{HOST}:{PORT}'.format(HOST=host, PORT=port)
         }
-        StandaloneApplication(app, options).run()
+        StandaloneApplication(current_app, options).run()
 
 
 # http://docs.gunicorn.org/en/latest/custom.html
 class StandaloneApplication(gunicorn.app.base.BaseApplication):
 
     def __init__(self, app, options=None):
         self.options = options or {}
```

### Comparing `lspace-0.4.5/lspace/file_types/_base.py` & `lspace-0.4.6/lspace/file_types/_base.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/file_types/epub.py` & `lspace-0.4.6/lspace/file_types/epub.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 
 class Epub(FileTypeBase):
     extension = '.epub'
 
     def __init__(self, path):
         super().__init__(path)
-        self.book = epub.read_epub(path)
+        # todo: ignore_ncx will default to true in next version,
+        # throws warning if not set
+        self.book = epub.read_epub(path, options=dict(ignore_ncx=True))
 
     def get_text(self):
         # type: () -> [str]
         text = []
 
         for doc in self.book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
             content = doc.get_content().decode('utf-8')
```

### Comparing `lspace-0.4.5/lspace/file_types/pdf.py` & `lspace-0.4.6/lspace/file_types/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 class PDF(FileTypeBase):
     extension = '.pdf'
 
     def __init__(self, path):
         super().__init__(path)
 
-        self.pdf_reader = pypdf.PdfFileReader(self.path)
-        self.metadata = self.pdf_reader.getDocumentInfo()
-        self.xmp_metadata = self.pdf_reader.getXmpMetadata()
+        self.pdf_reader = pypdf.PdfReader(self.path)
+        self.metadata = self.pdf_reader.metadata
+        self.xmp_metadata = self.pdf_reader.xmp_metadata
 
     def get_text(self):
         # type: () -> [str]
         pages = []
 
         # printing number of pages in pdf file
         for page_idx in range(min(self.pdf_reader.numPages, 30)):
```

### Comparing `lspace-0.4.5/lspace/frontend_blueprint/__init__.py` & `lspace-0.4.6/lspace/frontend_blueprint/__init__.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/frontend_blueprint/static/bulma.min.css` & `lspace-0.4.6/lspace/frontend_blueprint/static/bulma.min.css`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/frontend_blueprint/templates/base.html.jinja2` & `lspace-0.4.6/lspace/frontend_blueprint/templates/base.html.jinja2`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/frontend_blueprint/templates/books.html.jinja2` & `lspace-0.4.6/lspace/frontend_blueprint/templates/books.html.jinja2`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/frontend_blueprint/templates/macros.html.jinja2` & `lspace-0.4.6/lspace/frontend_blueprint/templates/macros.html.jinja2`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/helpers/__init__.py` & `lspace-0.4.6/lspace/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/helpers/init_logging.py` & `lspace-0.4.6/lspace/helpers/init_logging.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/helpers/query.py` & `lspace-0.4.6/lspace/helpers/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import isbnlib
 from typing import List
 
-from lspace import db
 from lspace.helpers import logger
 from lspace.models.meta_cache import MetaCache
 from lspace.models import Book, Author
 
 
 def _fetch_isbn_meta(isbn, service):
     try:
@@ -17,14 +16,15 @@
         meta = {}
     except Exception as e:
         logger.exception('failed to get isbn data from {service}: {error}'.format(error=e, service=service))
         meta = None
     return meta
 
 def _get_metadata_for_isbn(isbn, service='openl'):
+    from lspace.helpers.create_app import db
     # type: (str, str) -> Book
     cached_meta = MetaCache.query.filter_by(isbn=isbn, service=service).first()
     if cached_meta:
         meta = cached_meta.results
     else:
         meta = _fetch_isbn_meta(isbn, service)
         if meta != None:
```

### Comparing `lspace-0.4.5/lspace/migrations/env.py` & `lspace-0.4.6/lspace/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/migrations/versions/91732d5540b9_.py` & `lspace-0.4.6/lspace/migrations/versions/91732d5540b9_.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/migrations/versions/b142d6d9e8da_.py` & `lspace-0.4.6/lspace/migrations/versions/b142d6d9e8da_.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/migrations/versions/b9f9b5b4e882_.py` & `lspace-0.4.6/lspace/migrations/versions/b9f9b5b4e882_.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/migrations/versions/d8f2fb9f2472_.py` & `lspace-0.4.6/lspace/migrations/versions/d8f2fb9f2472_.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/migrations/versions/e2bbe7fd9bc7_.py` & `lspace-0.4.6/lspace/migrations/versions/e2bbe7fd9bc7_.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/models/author.py` & `lspace-0.4.6/lspace/models/author.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/models/book.py` & `lspace-0.4.6/lspace/models/book.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/models/book_author_association.py` & `lspace-0.4.6/lspace/models/book_author_association.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace/models/meta_cache.py` & `lspace-0.4.6/lspace/models/meta_cache.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/lspace.egg-info/PKG-INFO` & `lspace-0.4.6/lspace.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: lspace
-Version: 0.4.5
-Summary: a ebook manager built around isbnlib
+Version: 0.4.6
+Summary: ebook manager built around isbnlib
 Home-page: https://github.com/puhoy/lspace
 Author: jan
 Author-email: stuff@kwoh.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
-# L-Space
+# l-space
 
 a cli ebook manager built around [isbnlib](https://github.com/xlcnd/isbnlib)
 
-when importing it tries to find isbns in the files metadata and in the text. 
+on import, lspace tries to find isbns in the files metadata and in the text. 
 with the isbn it tries to fetch metadata about the book from google books and openlibrary. 
 if no isbn is found, it queries metadata based on the filename.
 
 after this, your properly renamed files will be stored in your library folder.
 
 currently supports epub and pdf.
 
@@ -235,9 +231,7 @@
 bumping is requires bump2version, twine is used for uploading to pypi.
 
 
 ## why "L-space"?
 
 its named after discworlds [library-space](https://en.wikipedia.org/wiki/List_of_dimensions_of_the_Discworld#L-space) dimension :)
 
-
-
```

### Comparing `lspace-0.4.5/lspace.egg-info/SOURCES.txt` & `lspace-0.4.6/lspace.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 lspace/__init__.py
-lspace/app.py
 lspace.egg-info/PKG-INFO
 lspace.egg-info/SOURCES.txt
 lspace.egg-info/dependency_links.txt
 lspace.egg-info/entry_points.txt
 lspace.egg-info/requires.txt
 lspace.egg-info/top_level.txt
 lspace/api_v1_blueprint/__init__.py
@@ -57,14 +56,15 @@
 lspace/frontend_blueprint/__init__.py
 lspace/frontend_blueprint/static/bulma.min.css
 lspace/frontend_blueprint/static/style.css
 lspace/frontend_blueprint/templates/base.html.jinja2
 lspace/frontend_blueprint/templates/books.html.jinja2
 lspace/frontend_blueprint/templates/macros.html.jinja2
 lspace/helpers/__init__.py
+lspace/helpers/create_app.py
 lspace/helpers/init_logging.py
 lspace/helpers/query.py
 lspace/migrations/README
 lspace/migrations/alembic.ini
 lspace/migrations/env.py
 lspace/migrations/script.py.mako
 lspace/migrations/versions/91732d5540b9_.py
```

### Comparing `lspace-0.4.5/lspace.egg-info/requires.txt` & `lspace-0.4.6/lspace.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-alembic==1.8.1
-aniso8601==8.0.0
-apispec==3.1.1
-attrs==19.3.0
-blinker==1.4
-certifi==2019.11.28
-chardet==3.0.4
-Click==8.0.3
-colorama==0.4.3
-EbookLib==0.17.1
-Flask==2.0.3
-Flask-Migrate==2.5.2
-flask-restx==0.5.1
-Flask-SQLAlchemy==2.5.1
-flask-whooshee==0.8.2
-Flask-WTF==1.0.0
+alembic==1.11.1
+aniso8601==9.0.1
+apispec==6.3.0
+attrs==23.1.0
+blinker==1.6.2
+certifi==2023.5.7
+chardet==5.1.0
+Click==8.1.4
+colorama==0.4.6
+EbookLib==0.18
+Flask==2.3.2
+Flask-Migrate==4.0.4
+flask-restx==1.1.0
+Flask-SQLAlchemy==3.0.5
+flask-whooshee==0.9.0
+Flask-WTF==1.1.1
 gunicorn==20.1.0
 html2text==2020.1.16
-idna==3.3
-isbnlib==3.10.9
-itsdangerous==2.0.1
-Jinja2==3.0.3
-jsonschema==3.2.0
-lxml==4.9.1
-Mako==1.1.0
-MarkupSafe==2.0.1
-marshmallow==3.14.1
-PyPDF2==1.27.5
-pyrsistent==0.15.6
-python-dateutil==2.8.1
+idna==3.4
+isbnlib==3.10.14
+itsdangerous==2.1.2
+Jinja2==3.1.2
+jsonschema==4.18.1
+lxml==4.9.3
+Mako==1.2.4
+MarkupSafe==2.1.3
+marshmallow==3.19.0
+PyPDF2==3.0.1
+pyrsistent==0.19.3
+python-dateutil==2.8.2
 python-editor==1.0.4
-python-slugify==4.0.0
-pytz==2021.3
-PyYAML==5.4
-requests==2.27.0
-six==1.13.0
-SQLAlchemy==1.4.31
+python-slugify==8.0.1
+pytz==2023.3
+PyYAML==6.0
+requests==2.31.0
+six==1.16.0
+SQLAlchemy==2.0.18
 text-unidecode==1.3
-typing==3.7.4.1
-urllib3==1.26.8
-Werkzeug==2.0.3
+typing==3.7.4.3
+urllib3==2.0.3
+Werkzeug==2.3.6
 Whoosh==2.7.4
 WTForms==3.0.1
 
 [dev]
-pytest==7.0.1
-pytest-cov==3.0.0
+pytest==7.4.0
+pytest-cov==4.1.0
 pytest-cover==3.0.0
-codecov==2.1.12
-ipython==8.0.1
-doit==0.34.1
-wheel==0.37.1
-twine==3.8.0
+codecov==2.1.13
+ipython==8.14.0
+doit==0.36.0
+wheel==0.40.0
+twine==4.0.2
+build==0.10.0
+bump2version==1.0.1
 
 [test]
-pytest==7.0.1
-pytest-cov==3.0.0
+pytest==7.4.0
+pytest-cov==4.1.0
 pytest-cover==3.0.0
-codecov==2.1.12
+codecov==2.1.13
```

### Comparing `lspace-0.4.5/tests/cli/_cli_test_base.py` & `lspace-0.4.6/tests/cli/_cli_test_base.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/tests/cli/import_command/test_calibre_meta_file.py` & `lspace-0.4.6/tests/cli/import_command/test_calibre_meta_file.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/tests/cli/import_command/test_copy_to_library.py` & `lspace-0.4.6/tests/cli/import_command/test_copy_to_library.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/tests/cli/test_list_command.py` & `lspace-0.4.6/tests/cli/test_list_command.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/tests/cli/tools/test_update_paths.py` & `lspace-0.4.6/tests/cli/tools/test_update_paths.py`

 * *Files identical despite different names*

### Comparing `lspace-0.4.5/tests/file_types/test_base.py` & `lspace-0.4.6/tests/file_types/test_base.py`

 * *Files identical despite different names*

