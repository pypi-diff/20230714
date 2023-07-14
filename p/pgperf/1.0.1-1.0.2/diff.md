# Comparing `tmp/pgperf-1.0.1.tar.gz` & `tmp/pgperf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgperf-1.0.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pgperf-1.0.1.tar` & `pgperf-1.0.2.tar`

### file list

```diff
@@ -1,125 +1,104 @@
--rw-r--r--   0        0        0    35148 2022-06-24 18:09:22.195604 pgperf-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0    21356 2022-06-23 08:52:18.893142 pgperf-1.0.1/README.rst
--rw-r--r--   0        0        0     1118 2022-06-24 18:18:57.237141 pgperf-1.0.1/long_description.md
--rw-r--r--   0        0        0     1013 2023-07-03 12:04:06.566941 pgperf-1.0.1/pgperf/__init__.py
--rw-r--r--   0        0        0     5321 2023-07-03 08:23:57.167777 pgperf-1.0.1/pgperf/db.py
--rw-r--r--   0        0        0      108 2023-07-03 11:55:47.681185 pgperf-1.0.1/pgperf/docs/index.md
--rw-r--r--   0        0        0      415 2023-07-03 11:09:56.003025 pgperf-1.0.1/pgperf/docs/pgperf/main.md
--rw-r--r--   0        0        0       32 2023-07-03 11:21:06.545659 pgperf-1.0.1/pgperf/index/__init__.py
--rw-r--r--   0        0        0     2576 2023-07-03 11:42:54.609857 pgperf-1.0.1/pgperf/index/main.py
--rw-r--r--   0        0        0     3456 2023-07-03 11:49:02.394295 pgperf-1.0.1/pgperf/main.py
--rw-r--r--   0        0        0       77 2023-07-03 11:41:20.883604 pgperf-1.0.1/pgperf/mkdocs.yml
--rw-r--r--   0        0        0      256 2023-07-03 11:09:29.850006 pgperf-1.0.1/pgperf/mkgendocs.yml
--rw-r--r--   0        0        0       33 2023-07-03 11:20:36.782634 pgperf-1.0.1/pgperf/server/__init__.py
--rw-r--r--   0        0        0      877 2023-06-30 22:48:00.639829 pgperf-1.0.1/pgperf/server/additional/__init__.py
--rw-r--r--   0        0        0     4810 2023-07-03 09:07:08.404802 pgperf-1.0.1/pgperf/server/configuration/__init__.py
--rw-r--r--   0        0        0     2300 2023-07-03 10:30:24.524361 pgperf-1.0.1/pgperf/server/configuration/replication.py
--rw-r--r--   0        0        0     1983 2023-07-03 11:16:19.662021 pgperf-1.0.1/pgperf/server/main.py
--rw-r--r--   0        0        0      659 2023-06-30 22:48:00.639829 pgperf-1.0.1/pgperf/server/stats/__init__.py
--rw-r--r--   0        0        0     8400 2023-07-03 10:26:15.010137 pgperf-1.0.1/pgperf/server/stats/collected.py
--rw-r--r--   0        0        0     2956 2023-06-30 22:11:39.798751 pgperf-1.0.1/pgperf/server/stats/dinamic.py
--rw-r--r--   0        0        0     3684 2023-07-03 11:58:07.810024 pgperf-1.0.1/pgperf/site/404.html
--rw-r--r--   0        0        0    87624 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-07-03 11:58:07.766692 pgperf-1.0.1/pgperf/site/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   129978 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/css/theme.css
--rw-r--r--   0        0        0     4597 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/css/theme_extra.css
--rw-r--r--   0        0        0     1150 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/img/favicon.ico
--rw-r--r--   0        0        0    28716 2023-07-03 11:58:07.826691 pgperf-1.0.1/pgperf/site/index.html
--rw-r--r--   0        0        0     2731 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/js/theme.js
--rw-r--r--   0        0        0      195 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/js/theme_extra.js
--rw-r--r--   0        0        0     5096 2023-07-03 11:58:07.826691 pgperf-1.0.1/pgperf/site/pgperf/main/index.html
--rw-r--r--   0        0        0    99805 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/search/lunr.js
--rw-r--r--   0        0        0     3206 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/search/main.js
--rw-r--r--   0        0        0    32902 2023-07-03 11:58:07.826691 pgperf-1.0.1/pgperf/site/search/search_index.json
--rw-r--r--   0        0        0     3724 2023-07-03 11:58:07.770025 pgperf-1.0.1/pgperf/site/search/worker.js
--rw-r--r--   0        0        0     4159 2023-07-03 11:58:07.816691 pgperf-1.0.1/pgperf/site/search.html
--rw-r--r--   0        0        0      109 2023-07-03 11:58:07.813358 pgperf-1.0.1/pgperf/site/sitemap.xml
--rw-r--r--   0        0        0      127 2023-07-03 11:58:07.813358 pgperf-1.0.1/pgperf/site/sitemap.xml.gz
--rw-r--r--   0        0        0       32 2023-07-03 11:36:01.363334 pgperf-1.0.1/pgperf/table/__init__.py
--rw-r--r--   0        0        0     2237 2023-07-03 11:44:49.252585 pgperf-1.0.1/pgperf/table/main.py
--rw-r--r--   0        0        0      527 2022-06-21 14:26:49.783784 pgperf-1.0.1/pgperf/templates/all_locks.sql
--rw-r--r--   0        0        0     4124 2022-06-21 14:26:49.783784 pgperf-1.0.1/pgperf/templates/bloat.sql
--rw-r--r--   0        0        0      553 2022-06-21 14:26:49.783784 pgperf-1.0.1/pgperf/templates/blocking.sql
--rw-r--r--   0        0        0      691 2022-06-21 14:26:49.783784 pgperf-1.0.1/pgperf/templates/buffercache_stats.sql
--rw-r--r--   0        0        0      350 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/buffercache_usage.sql
--rw-r--r--   0        0        0      328 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/cache_hit.sql
--rw-r--r--   0        0        0      564 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/calls.sql
--rw-r--r--   0        0        0      549 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/calls_legacy.sql
--rw-r--r--   0        0        0      656 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/duplicate_indexes.sql
--rw-r--r--   0        0        0      499 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/index_cache_hit.sql
--rw-r--r--   0        0        0      434 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/index_scans.sql
--rw-r--r--   0        0        0      378 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/index_size.sql
--rw-r--r--   0        0        0      319 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/index_usage.sql
--rw-r--r--   0        0        0      278 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/indexes.sql
--rw-r--r--   0        0        0      653 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/locks.sql
--rw-r--r--   0        0        0      357 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/long_running_queries.sql
--rw-r--r--   0        0        0     1120 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/null_indexes.sql
--rw-r--r--   0        0        0      591 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/outliers.sql
--rw-r--r--   0        0        0      123 2023-06-30 09:09:21.620176 pgperf-1.0.1/pgperf/templates/pg_stat_statements_reset.sql
--rw-r--r--   0        0        0      193 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/records_rank.sql
--rw-r--r--   0        0        0      155 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/seq_scans.sql
--rw-r--r--   0        0        0      233 2022-06-21 14:26:49.783784 pgperf-1.0.1/pgperf/templates/server/active_conection.sql
--rw-r--r--   0        0        0      200 2023-06-30 22:33:18.023676 pgperf-1.0.1/pgperf/templates/server/additional/add_all_recommended_extensions.sql
--rw-r--r--   0        0        0      106 2023-06-30 22:33:28.616938 pgperf-1.0.1/pgperf/templates/server/additional/extensions.sql
--rw-r--r--   0        0        0        9 2023-07-01 20:52:32.207657 pgperf-1.0.1/pgperf/templates/server/config/show_all.sql
--rw-r--r--   0        0        0       20 2023-07-03 08:22:50.138713 pgperf-1.0.1/pgperf/templates/server/config/show_variable.sql
--rw-r--r--   0        0        0      483 2023-07-01 20:54:10.413036 pgperf-1.0.1/pgperf/templates/server/db_settings.sql
--rw-r--r--   0        0        0      213 2022-06-21 14:26:49.787117 pgperf-1.0.1/pgperf/templates/server/kill_all.sql
--rw-r--r--   0        0        0       59 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/server/ssl_used.sql
--rw-r--r--   0        0        0       34 2023-06-30 21:31:28.179266 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_all_indexes.sql
--rw-r--r--   0        0        0       33 2023-06-30 21:30:05.484644 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_all_tables.sql
--rw-r--r--   0        0        0       31 2023-06-30 21:25:48.657476 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_archiver.sql
--rw-r--r--   0        0        0       31 2023-06-30 21:29:11.240477 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_bgwriter.sql
--rw-r--r--   0        0        0       30 2023-06-30 21:29:31.820792 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_database.sql
--rw-r--r--   0        0        0       41 2023-06-30 21:29:52.481110 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_database_conflicts.sql
--rw-r--r--   0        0        0       34 2023-06-30 21:31:54.886353 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_sys_indexes.sql
--rw-r--r--   0        0        0       33 2023-06-30 21:30:21.371556 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_sys_tables.sql
--rw-r--r--   0        0        0       37 2023-06-30 21:35:31.171649 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_user_functions.sql
--rw-r--r--   0        0        0       35 2023-06-30 21:32:12.206627 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_user_indexes.sql
--rw-r--r--   0        0        0       34 2023-06-30 21:30:35.798447 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_user_tables.sql
--rw-r--r--   0        0        0       38 2023-06-30 21:30:46.171942 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_xact_all_tables.sql
--rw-r--r--   0        0        0       38 2023-06-30 21:31:00.458831 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_xact_sys_tables.sql
--rw-r--r--   0        0        0       42 2023-06-30 21:35:46.177137 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_xact_user_functions.sql
--rw-r--r--   0        0        0       39 2023-06-30 21:31:14.405717 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_stat_xact_user_tables.sql
--rw-r--r--   0        0        0       36 2023-06-30 21:33:36.688508 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_all_indexes.sql
--rw-r--r--   0        0        0       38 2023-06-30 21:34:47.728590 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_all_sequences.sql
--rw-r--r--   0        0        0       35 2023-06-30 21:32:24.903495 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_all_tables.sql
--rw-r--r--   0        0        0       36 2023-06-30 21:33:31.978977 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_sys_indexes.sql
--rw-r--r--   0        0        0       38 2023-06-30 21:35:02.374007 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_sys_sequences.sql
--rw-r--r--   0        0        0       37 2023-06-30 21:33:38.654980 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_sys_tables.sql
--rw-r--r--   0        0        0       37 2023-06-30 21:34:28.086988 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_user_indexes.sql
--rw-r--r--   0        0        0       39 2023-06-30 21:35:17.672738 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_user_sequences.sql
--rw-r--r--   0        0        0       36 2023-06-30 21:32:56.180660 pgperf-1.0.1/pgperf/templates/server/stats/collected/pg_statio_user_tables.sql
--rw-r--r--   0        0        0       31 2023-06-30 09:09:41.996661 pgperf-1.0.1/pgperf/templates/server/stats/dinamic/pg_stat_activity.sql
--rw-r--r--   0        0        0       38 2023-06-30 10:05:58.057835 pgperf-1.0.1/pgperf/templates/server/stats/dinamic/pg_stat_progress_vacuum.sql
--rw-r--r--   0        0        0       34 2023-06-30 09:26:54.710612 pgperf-1.0.1/pgperf/templates/server/stats/dinamic/pg_stat_replication.sql
--rw-r--r--   0        0        0       26 2023-06-30 09:55:36.786742 pgperf-1.0.1/pgperf/templates/server/stats/dinamic/pg_stat_ssl.sql
--rw-r--r--   0        0        0       34 2023-06-30 09:52:44.191723 pgperf-1.0.1/pgperf/templates/server/stats/dinamic/pg_stat_subscription.sql
--rw-r--r--   0        0        0       34 2023-06-30 09:47:04.234986 pgperf-1.0.1/pgperf/templates/server/stats/dinamic/pg_stat_wal_receiver.sql
--rw-r--r--   0        0        0     1918 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/server/vacuum_stats.sql
--rw-r--r--   0        0        0      510 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/table_cache_hit.sql
--rw-r--r--   0        0        0      179 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/table_index_scans.sql
--rw-r--r--   0        0        0      389 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/table_index_size.sql
--rw-r--r--   0        0        0      373 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/table_size.sql
--rw-r--r--   0        0        0      298 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/total_index_size.sql
--rw-r--r--   0        0        0      391 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/total_table_size.sql
--rw-r--r--   0        0        0      734 2022-06-21 14:26:49.790451 pgperf-1.0.1/pgperf/templates/unused_indexes.sql
--rw-r--r--   0        0        0     1584 2023-07-03 12:04:11.240233 pgperf-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 pgperf-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pgperf-1.0.2/.envrc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pgperf-1.0.2/.projectile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pgperf-1.0.2/.tool-versions
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pgperf-1.0.2/long_description.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pgperf-1.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pgperf-1.0.2/mkgendocs.yml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pgperf-1.0.2/pgperf.code-workspace
+-rw-r--r--   0        0        0   179507 2020-02-02 00:00:00.000000 pgperf-1.0.2/poetry.lock
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pgperf-1.0.2/docs/index.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/__version__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/db.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/pgperf.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/index/__init__.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/index/main.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/__init__.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/main.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/additional/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/configuration/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/configuration/replication.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/stats/__init__.py
+-rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/stats/collected.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/server/stats/dinamic.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/table/__init__.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/table/main.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/all_locks.sql
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/blocking.sql
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/buffercache_stats.sql
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/buffercache_usage.sql
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/locks.sql
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/long_running_queries.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/pg_stat_statements_reset.sql
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/cache_hit.sql
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/duplicate_indexes.sql
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/index_cache_hit.sql
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/index_scans.sql
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/index_size.sql
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/index_usage.sql
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/indexes.sql
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/null_indexes.sql
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/total_index_size.sql
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/index/unused_indexes.sql
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/active_conection.sql
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/db_settings.sql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/kill_all.sql
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/ssl_used.sql
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/vacuum_stats.sql
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/additional/add_all_recommended_extensions.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/additional/extensions.sql
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/config/show_all.sql
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/config/show_variable.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_all_indexes.sql
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_all_tables.sql
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_archiver.sql
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_bgwriter.sql
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_database.sql
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_database_conflicts.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_sys_indexes.sql
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_sys_tables.sql
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_user_functions.sql
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_user_indexes.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_user_tables.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_xact_all_tables.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_xact_sys_tables.sql
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_xact_user_functions.sql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_stat_xact_user_tables.sql
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_all_indexes.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_all_sequences.sql
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_all_tables.sql
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_sys_indexes.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_sys_sequences.sql
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_sys_tables.sql
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_user_indexes.sql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_user_sequences.sql
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/collected/pg_statio_user_tables.sql
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/dinamic/pg_stat_activity.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/dinamic/pg_stat_progress_vacuum.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/dinamic/pg_stat_replication.sql
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/dinamic/pg_stat_ssl.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/dinamic/pg_stat_subscription.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/server/stats/dinamic/pg_stat_wal_receiver.sql
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/bloat.sql
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/records_rank.sql
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/seq_scans.sql
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/table_cache_hit.sql
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/table_index_scans.sql
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/table_index_size.sql
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/table_size.sql
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pgperf-1.0.2/src/pgperf/templates/table/total_table_size.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_index.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_server.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_server_additional.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_server_configuration.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_server_configuration_replication.py
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_server_stats_collected.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_server_stats_dinanic.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pgperf-1.0.2/tests/test_pgperf_table.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pgperf-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pgperf-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0    31989 2020-02-02 00:00:00.000000 pgperf-1.0.2/README.md
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 pgperf-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 pgperf-1.0.2/PKG-INFO
```

### Comparing `pgperf-1.0.1/LICENSE.txt` & `pgperf-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/__init__.py` & `pgperf-1.0.2/src/pgperf/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-__version__ = '1.0.1'
-
 import os
 from rich.console import Console
 from omegaconf import OmegaConf
 from jinja2 import Environment, PackageLoader
 
 console = Console()
 user_home = os.path.expanduser('~')
```

### Comparing `pgperf-1.0.1/pgperf/index/main.py` & `pgperf-1.0.2/src/pgperf/index/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pgperf import console, config
 from pgperf.db import Db
 import typer
 
 app = typer.Typer()
 
-state = {"conf": config['prod'], "path": "server/"}
+state = {"conf": config['prod'], "path": "index/"}
 
 
 @app.callback()
 def main(verbose: bool = False, debug: bool = False, conf: str = ""):
     """
     Index Informations 
     """
@@ -18,95 +18,95 @@
 
 @app.command()
 def duplicate():
     """
     Show multiple indexes that have the same set of columns, same opclass, expression and predicate.
     """
     db = Db(state['conf'])
-    result = db.duplicate_indexes()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'duplicate_indexes')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def cache_hit():
     """
     Calculates your cache hit rate for reading indexes
     """
     db = Db(state['conf'])
-    result = db.index_cache_hit()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'index_cache_hit')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def scans():
     """
     Number of scans performed on indexes
     """
     db = Db(state['conf'])
-    result = db.index_scans()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'index_scans')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def size():
     """
     The size of indexes, descending by size, in MB.
     """
     db = Db(state['conf'])
-    result = db.index_size()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'index_size')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def usage():
     """
     Index hit rate (effective databases are at 99% and up)
     """
     db = Db(state['conf'])
-    result = db.index_usage()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'index_usage')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def null():
     """
     Find indexes with a high ratio of NULL values
     """
     db = Db(state['conf'])
-    result = db.null_indexes()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'null_indexes')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def total_size():
     """
     Total size of all indexes in MB
     """
     db = Db(state['conf'])
-    result = db.total_index_size()
+    result = db.get_from_path(state['path'], 'total_index_size')
     console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def unused():
     """
     Unused and almost unused indexes. Ordered by their size relative to the number of index scans.
     Exclude indexes of very small tables (less than 5 pages), where the planner will almost invariably select a sequential scan,
     but may not in the future as the table grows
     """
     db = Db(state['conf'])
-    result = db.unused_indexes()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'unused_indexes')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def all():
     """
     List all the indexes with their corresponding tables and columns.
     """
     db = Db(state['conf'])
-    result = db.indexes()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'indexes')
+    console.print(result.to_markdown(), justify="left")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pgperf-1.0.1/pgperf/main.py` & `pgperf-1.0.2/src/pgperf/pgperf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from pgperf import console, config, __version__
-from pgperf.db import Db
-from pgperf.server import app as server_app
-from pgperf.index import app as index_app
-from pgperf.table import app as table_app
-import pandas as pd
 import typer
+from pgperf.table import app as table_app
+from pgperf.index import app as index_app
+from pgperf.server import app as server_app
+from pgperf.db import Db
+from pgperf.__version__ import __version__
+from pgperf import console, config
+
 
 app = typer.Typer()
 app.add_typer(server_app, name="server")
 app.add_typer(index_app, name="index")
 app.add_typer(table_app, name="table")
 
-state = {"conf": config['prod']}
+state = {"conf": config['prod'], "path": ""}
 
 
 @app.callback()
 def main(conf: str = ""):
     """
     Python port of [Heroku PG Extras](https://github.com/heroku/heroku-pg-extras) with several additions and improvements.
 
@@ -26,119 +27,74 @@
 
 
 @app.command()
 def all_locks():
     """
     List all current locks in your database
     """
-    if state['verbose']:
-        console.rule("[bold] All the current locks")
     db = Db(state['conf'])
-    result = db.all_locks()
+    result = db.get_from_path(state['path'], 'all_locks')
     console.print(result.to_markdown(), justify="center")
 
 
 @app.command()
 def blocking():
     """
     Get all statements that are currently holding locks in your database
     """
     db = Db(state['conf'])
-    result = db.blocking()
+    result = db.get_from_path(state['path'], 'blocking')
     console.print(result.to_markdown(), justify="center")
 
 
 @app.command()
 def buffercache_stats():
     """
     Get all Buffercache Stats
     """
     db = Db(state['conf'])
-    result = db.buffercache_stats()
+    result = db.get_from_path(state['path'], 'buffercache_stats')
     console.print(result.to_markdown(), justify="center")
 
 
 @app.command()
 def buffercache_usage():
     """
     Get all Buffercache Usage
     """
     db = Db(state['conf'])
-    result = db.buffercache_usage()
+    result = db.get_from_path(state['path'], 'buffercache_usage')
     console.print(result.to_markdown(), justify="center")
 
 
 @app.command()
-def cache_hits():
-    """
-    Get all cache hits
-    """
-    db = Db(state['conf'])
-    result = db.cache_hit()
-    console.print(result.to_markdown(), justify="center")
-
-
-@app.command()
-def calls_legacy():
-    """
-    Get the queries that have highest frequency of execution
-    """
-    # TODO: Pendind test and validate
-    db = Db(state['conf'])
-    result = db.calls_legacy()
-    console.print(result.to_markdown())
-
-
-@app.command()
-def calls():
-    """
-    Get the queries that have highest frequency of execution
-    """
-    db = Db(state['conf'])
-    result = db.calls()
-    console.print(result.to_markdown())
-
-
-@app.command()
 def locks():
     """
     Queries with active exclusive locks
     """
     db = Db(state['conf'])
-    result = db.locks()
+    result = db.get_from_path(state['path'], 'locks')
     console.print(result.to_markdown(), justify="center")
 
 
 @app.command()
 def long_running_queries():
     """
     All queries longer than five minutes by descending duration
     """
     db = Db(state['conf'])
-    result = db.long_running_queries()
+    result = db.get_from_path(state['path'], 'long_running_queries')
     console.print(result.to_markdown(), justify="center")
 
 
 @app.command()
-def outliers():
-    """
-    Queries that have longest execution time in aggregate
-    """
-    db = Db(state['conf'])
-    result = db.outliers()
-    console.print(result.to_markdown())
+def version():
+    console.print(__version__)
 
 
 @app.command()
-def version():
-    console.rule("[bold red]PG Extras APP", align="center")
-    console.print()
-    console.print(
-        "[bold] Postgresql Extras APP", justify="center")
-    console.print(f"Installed version => {__version__}", justify="center")
-    console.print(f"Connected to ==> {config}", justify="center")
-    console.print()
-    console.rule("[bold red]..::==> Thanks <==::..")
+def show_config():
+    console.print(state['conf'])
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pgperf-1.0.1/pgperf/server/additional/__init__.py` & `pgperf-1.0.2/src/pgperf/server/additional/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 app = typer.Typer()
 
 state = {"conf": config['prod'], "path": "server/additional/"}
 
 
 @app.callback()
-def main(verbose: bool = False, debug: bool = False, conf: str = ""):
+def main(conf: str = ""):
     """
     Additional Supplied Modules 
     """
     if conf:
         state['conf'] = config[conf]
 
 
@@ -28,13 +28,13 @@
 
 @app.command()
 def add_all_recommended_extensions():
     """
     Adding Extensions [sslinfo, pg_buffercache, pg_stat_statements] to your database.
     """
     db = Db(state['conf'])
-    db.exec_from_path(state['path'], "add_al")
-    db.add_extensions()
+    db.exec_from_path(state['path'], "add_all_recommended_extensions")
+    extensions()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pgperf-1.0.1/pgperf/server/configuration/__init__.py` & `pgperf-1.0.2/src/pgperf/server/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/server/configuration/replication.py` & `pgperf-1.0.2/src/pgperf/server/configuration/replication.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         result = db.get_from_path_with_var(
             state['path'], "show_variable", conf)
         data[conf] = result.iloc[0][conf]
     return data
 
 
 @app.callback()
-def main(verbose: bool = False, debug: bool = False, conf: str = ""):
+def main(conf: str = ""):
     """
     Server Replication information
     """
     if conf:
         state['conf'] = config[conf]
```

### Comparing `pgperf-1.0.1/pgperf/server/main.py` & `pgperf-1.0.2/src/pgperf/server/main.py`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/server/stats/__init__.py` & `pgperf-1.0.2/src/pgperf/server/stats/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 app = typer.Typer()
 app.add_typer(dinamic_app, name="dinamic")
 app.add_typer(collected_app, name="collected")
 state = {"conf": config['prod']}
 
 
 @app.callback()
-def main(verbose: bool = False, debug: bool = False, conf: str = ""):
+def main(conf: str = ""):
     """
     The Statistics Collector.
     PostgreSQL's statistics collector is a subsystem that supports collection and reporting of information about server activity. 
     """
     if conf:
         state['conf'] = config[conf]
```

### Comparing `pgperf-1.0.1/pgperf/server/stats/collected.py` & `pgperf-1.0.2/src/pgperf/server/stats/collected.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typer
 
 app = typer.Typer()
 state = {"conf": config['prod'], "path": "server/stats/collected/"}
 
 
 @app.callback()
-def collected(verbose: bool = False, debug: bool = False, conf: str = ""):
+def collected(conf: str = ""):
     """
     Collected Statistics Views 
     """
     if conf:
         state['conf'] = config[conf]
```

### Comparing `pgperf-1.0.1/pgperf/server/stats/dinamic.py` & `pgperf-1.0.2/src/pgperf/server/stats/dinamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typer
 
 app = typer.Typer()
 state = {"conf": config['prod'], "path": "server/stats/dinamic/"}
 
 
 @app.callback()
-def main(verbose: bool = False, debug: bool = False, conf: str = ""):
+def main(conf: str = ""):
     """
     Dynamic Statistics Views 
     """
     if conf:
         state['conf'] = config[conf]
 
 
@@ -82,20 +82,9 @@
     running VACUUM, showing current progress. ( >= PostgresSQL  11.0 )
     """
     db = Db(state['conf'])
     result = db.get_from_path(state['path'], "pg_stat_progress_vacuum")
     console.print(result.to_markdown(), justify="left")
 
 
-@app.command()
-def statements_reset():
-    """
-    pg_stat_statements_reset discards statistics gathered so far by 
-    pg_stat_statements ( >= PostgresSQL  11.0 )
-    """
-    db = Db(state['conf'])
-    result = db.get_from_path(state['path'], "pg_stat_statements_reset")
-    console.print(result.to_markdown(), justify="center")
-
-
 if __name__ == "__main__":
     app()
```

### Comparing `pgperf-1.0.1/pgperf/table/main.py` & `pgperf-1.0.2/src/pgperf/table/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pgperf import console, config
 from pgperf.db import Db
 import typer
 
 app = typer.Typer()
 
-state = {"conf": config['prod'], "path": "server/"}
+state = {"conf": config['prod'], "path": "table/"}
 
 
 @app.callback()
 def main(verbose: bool = False, debug: bool = False, conf: str = ""):
     """
     Table Informations 
     """
@@ -18,82 +18,83 @@
 
 @app.command()
 def records_rank():
     """
     All tables and the number of rows in each ordered by number of rows descending
     """
     db = Db(state['conf'])
-    result = db.records_rank()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'records_rank')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def seq_scans():
     """
     Count of sequential scans by table descending by order
     """
     db = Db(state['conf'])
-    result = db.seq_scans()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'seq_scans')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def cache_hit():
     """
     Calculates your cache hit rate for reading tables
     """
     db = Db(state['conf'])
-    result = db.table_cache_hit()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'table_cache_hit')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def index_scans():
     """
     Count of index scans by table descending by order
     """
     db = Db(state['conf'])
-    result = db.table_index_scans()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'table_index_scans')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def index_size():
     """
     Total size of all the indexes on each table, descending by size
     """
     db = Db(state['conf'])
-    result = db.table_index_size()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'table_index_size')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def size():
     """
     Size of the tables (excluding indexes), descending by size
     """
     db = Db(state['conf'])
-    result = db.table_size()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'table_size')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def size_with_index():
     """
     Size of the tables (including indexes), descending by size
     """
     db = Db(state['conf'])
-    result = db.total_table_size()
-    console.print(result.to_markdown(), justify="center")
+    result = db.get_from_path(state['path'], 'total_table_size')
+    console.print(result.to_markdown(), justify="left")
 
 
 @app.command()
 def bloat():
     """
     Estimation of table 'bloat' space allocated to a relation that is full of dead tuples, that has yet to be reclaimed.
     """
-    result = db.bloat()
-    console.print(result.to_markdown(), justify="center")
+    db = Db(state['conf'])
+    result = db.get_from_path(state['path'], 'bloat')
+    console.print(result.to_markdown(), justify="left")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pgperf-1.0.1/pgperf/templates/all_locks.sql` & `pgperf-1.0.2/src/pgperf/templates/all_locks.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/bloat.sql` & `pgperf-1.0.2/src/pgperf/templates/table/bloat.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/blocking.sql` & `pgperf-1.0.2/src/pgperf/templates/blocking.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/buffercache_stats.sql` & `pgperf-1.0.2/src/pgperf/templates/buffercache_stats.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/duplicate_indexes.sql` & `pgperf-1.0.2/src/pgperf/templates/index/duplicate_indexes.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/locks.sql` & `pgperf-1.0.2/src/pgperf/templates/locks.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/null_indexes.sql` & `pgperf-1.0.2/src/pgperf/templates/index/null_indexes.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/server/vacuum_stats.sql` & `pgperf-1.0.2/src/pgperf/templates/server/vacuum_stats.sql`

 * *Files identical despite different names*

### Comparing `pgperf-1.0.1/pgperf/templates/unused_indexes.sql` & `pgperf-1.0.2/src/pgperf/templates/index/unused_indexes.sql`

 * *Files identical despite different names*

