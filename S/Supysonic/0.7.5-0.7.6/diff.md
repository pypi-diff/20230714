# Comparing `tmp/Supysonic-0.7.5.tar.gz` & `tmp/Supysonic-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Supysonic-0.7.5.tar", last modified: Sun Apr  2 14:19:05 2023, max compression
+gzip compressed data, was "Supysonic-0.7.6.tar", last modified: Fri Jul 14 13:28:33 2023, max compression
```

## Comparing `Supysonic-0.7.5.tar` & `Supysonic-0.7.6.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:04.847364 Supysonic-0.7.5/
--rw-rw-rw-   0        0        0    34520 2021-01-23 14:44:54.000000 Supysonic-0.7.5/LICENSE
--rw-rw-rw-   0        0        0      154 2021-12-19 16:15:13.000000 Supysonic-0.7.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1712 2023-04-02 14:19:03.465554 Supysonic-0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     2738 2023-02-11 13:36:47.000000 Supysonic-0.7.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.385584 Supysonic-0.7.5/Supysonic.egg-info/
--rw-rw-rw-   0        0        0     1712 2023-04-02 14:19:03.000000 Supysonic-0.7.5/Supysonic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4802 2023-04-02 14:19:03.000000 Supysonic-0.7.5/Supysonic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 14:19:03.000000 Supysonic-0.7.5/Supysonic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-04-02 14:19:03.000000 Supysonic-0.7.5/Supysonic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-12-31 16:33:42.000000 Supysonic-0.7.5/Supysonic.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-04-02 14:19:03.000000 Supysonic-0.7.5/Supysonic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-02 14:19:03.000000 Supysonic-0.7.5/Supysonic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3005 2023-03-18 14:41:06.000000 Supysonic-0.7.5/config.sample
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:05.255454 Supysonic-0.7.5/man/
--rw-rw-rw-   0        0        0     3675 2023-04-02 14:19:05.201750 Supysonic-0.7.5/man/supysonic-cli-folder.1
--rw-rw-rw-   0        0        0     4128 2023-04-02 14:19:05.185784 Supysonic-0.7.5/man/supysonic-cli-user.1
--rw-rw-rw-   0        0        0     2769 2023-04-02 14:19:05.180735 Supysonic-0.7.5/man/supysonic-cli.1
--rw-rw-rw-   0        0        0     1852 2023-04-02 14:19:05.205790 Supysonic-0.7.5/man/supysonic-daemon.1
--rw-rw-rw-   0        0        0     2984 2023-04-02 14:19:05.205790 Supysonic-0.7.5/man/supysonic-server.1
--rw-rw-rw-   0        0        0      108 2022-04-23 14:58:53.000000 Supysonic-0.7.5/pyproject.toml
--rw-rw-rw-   0        0        0     2175 2023-04-02 14:19:03.465554 Supysonic-0.7.5/setup.cfg
--rw-rw-rw-   0        0        0      763 2022-04-23 14:58:53.000000 Supysonic-0.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.395580 Supysonic-0.7.5/supysonic/
--rw-rw-rw-   0        0        0      534 2023-04-02 14:01:55.000000 Supysonic-0.7.5/supysonic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.405613 Supysonic-0.7.5/supysonic/api/
--rw-rw-rw-   0        0        0     3762 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/__init__.py
--rw-rw-rw-   0        0        0     9758 2023-03-18 16:38:26.000000 Supysonic-0.7.5/supysonic/api/albums_songs.py
--rw-rw-rw-   0        0        0     4941 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/annotation.py
--rw-rw-rw-   0        0        0     5690 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/api/browse.py
--rw-rw-rw-   0        0        0      856 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/chat.py
--rw-rw-rw-   0        0        0     1035 2023-02-25 16:35:07.000000 Supysonic-0.7.5/supysonic/api/errors.py
--rw-rw-rw-   0        0        0     3585 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/exceptions.py
--rw-rw-rw-   0        0        0     5165 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/formatters.py
--rw-rw-rw-   0        0        0     2625 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/jukebox.py
--rw-rw-rw-   0        0        0    15944 2023-03-18 14:45:11.000000 Supysonic-0.7.5/supysonic/api/media.py
--rw-rw-rw-   0        0        0     3394 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/playlists.py
--rw-rw-rw-   0        0        0     1878 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/radio.py
--rw-rw-rw-   0        0        0     1367 2021-11-28 15:13:37.000000 Supysonic-0.7.5/supysonic/api/scan.py
--rw-rw-rw-   0        0        0     6948 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/search.py
--rw-rw-rw-   0        0        0      434 2021-11-28 15:13:37.000000 Supysonic-0.7.5/supysonic/api/system.py
--rw-rw-rw-   0        0        0      661 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/unsupported.py
--rw-rw-rw-   0        0        0     2883 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/api/user.py
--rw-rw-rw-   0        0        0     7911 2021-01-23 14:44:54.000000 Supysonic-0.7.5/supysonic/cache.py
--rw-rw-rw-   0        0        0     9754 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/cli.py
--rw-rw-rw-   0        0        0     2708 2023-03-18 14:41:06.000000 Supysonic-0.7.5/supysonic/config.py
--rw-rw-rw-   0        0        0     2070 2022-01-30 15:22:37.000000 Supysonic-0.7.5/supysonic/covers.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.405613 Supysonic-0.7.5/supysonic/daemon/
--rw-rw-rw-   0        0        0     1668 2023-03-18 11:40:04.000000 Supysonic-0.7.5/supysonic/daemon/__init__.py
--rw-rw-rw-   0        0        0      259 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/daemon/__main__.py
--rw-rw-rw-   0        0        0     5313 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/daemon/client.py
--rw-rw-rw-   0        0        0      252 2021-01-23 14:44:54.000000 Supysonic-0.7.5/supysonic/daemon/exceptions.py
--rw-rw-rw-   0        0        0     3620 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/daemon/server.py
--rw-rw-rw-   0        0        0    20172 2023-04-02 13:37:21.000000 Supysonic-0.7.5/supysonic/db.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.405613 Supysonic-0.7.5/supysonic/frontend/
--rw-rw-rw-   0        0        0     2382 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/frontend/__init__.py
--rw-rw-rw-   0        0        0     2747 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/frontend/folder.py
--rw-rw-rw-   0        0        0     2627 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/frontend/playlist.py
--rw-rw-rw-   0        0        0     9161 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/frontend/user.py
--rw-rw-rw-   0        0        0     4204 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/jukebox.py
--rw-rw-rw-   0        0        0     3519 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/lastfm.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.405613 Supysonic-0.7.5/supysonic/managers/
--rw-rw-rw-   0        0        0      200 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/managers/__init__.py
--rw-rw-rw-   0        0        0     2173 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/managers/folder.py
--rw-rw-rw-   0        0        0     2528 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/managers/user.py
--rw-rw-rw-   0        0        0    12971 2023-04-01 16:45:47.000000 Supysonic-0.7.5/supysonic/scanner.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.415576 Supysonic-0.7.5/supysonic/schema/
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.375453 Supysonic-0.7.5/supysonic/schema/migration/
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.425583 Supysonic-0.7.5/supysonic/schema/migration/mysql/
--rw-rw-rw-   0        0        0      292 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20161030.sql
--rw-rw-rw-   0        0        0      227 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20171022.sql
--rw-rw-rw-   0        0        0     2758 2023-01-08 15:12:52.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20171230.py
--rw-rw-rw-   0        0        0     3030 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20180221.sql
--rw-rw-rw-   0        0        0      386 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20180317.sql
--rw-rw-rw-   0        0        0      208 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20180521.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20181010.sql
--rw-rw-rw-   0        0        0     1452 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20190324.sql
--rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20190518.sql
--rw-rw-rw-   0        0        0     2767 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20190915.sql
--rw-rw-rw-   0        0        0       73 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20190921.sql
--rw-rw-rw-   0        0        0      266 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20200607.sql
--rw-rw-rw-   0        0        0     2745 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20230111.py
--rw-rw-rw-   0        0        0      155 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20230115.sql
--rw-rw-rw-   0        0        0       88 2023-04-02 13:50:59.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/20230331.sql
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.425583 Supysonic-0.7.5/supysonic/schema/migration/mysql/__pycache__/
--rw-rw-rw-   0        0        0     2400 2023-01-11 21:50:42.000000 Supysonic-0.7.5/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.425583 Supysonic-0.7.5/supysonic/schema/migration/postgres/
--rw-rw-rw-   0        0        0      267 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20161030.sql
--rw-rw-rw-   0        0        0      232 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20171022.sql
--rw-rw-rw-   0        0        0      229 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20180311.sql
--rw-rw-rw-   0        0        0     1136 2023-01-08 15:12:52.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20180317.py
--rw-rw-rw-   0        0        0      188 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20180521.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20181010.sql
--rw-rw-rw-   0        0        0     1748 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20190324.sql
--rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20190518.sql
--rw-rw-rw-   0        0        0     3649 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20190915.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20190921.sql
--rw-rw-rw-   0        0        0      204 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20200607.sql
--rw-rw-rw-   0        0        0      153 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20230115.sql
--rw-rw-rw-   0        0        0       88 2023-04-02 13:50:59.000000 Supysonic-0.7.5/supysonic/schema/migration/postgres/20230331.sql
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.435575 Supysonic-0.7.5/supysonic/schema/migration/sqlite/
--rw-rw-rw-   0        0        0     1176 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20161030.sql
--rw-rw-rw-   0        0        0      882 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20171022.sql
--rw-rw-rw-   0        0        0     2032 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20171230.py
--rw-rw-rw-   0        0        0     1629 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20180311.sql
--rw-rw-rw-   0        0        0      939 2023-01-08 15:12:52.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20180317.py
--rw-rw-rw-   0        0        0      754 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20180521.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20181010.sql
--rw-rw-rw-   0        0        0     1746 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20190324.sql
--rw-rw-rw-   0        0        0     1858 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20190518.sql
--rw-rw-rw-   0        0        0     5084 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20190915.sql
--rw-rw-rw-   0        0        0       61 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20190921.sql
--rw-rw-rw-   0        0        0      207 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20200607.sql
--rw-rw-rw-   0        0        0     1924 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20230111.py
--rw-rw-rw-   0        0        0      499 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20230115.sql
--rw-rw-rw-   0        0        0       87 2023-04-02 13:50:59.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/20230331.sql
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.435575 Supysonic-0.7.5/supysonic/schema/migration/sqlite/__pycache__/
--rw-rw-rw-   0        0        0     1743 2023-02-11 13:37:00.000000 Supysonic-0.7.5/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc
--rw-rw-rw-   0        0        0     6463 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/mysql.sql
--rw-rw-rw-   0        0        0     5689 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/postgres.sql
--rw-rw-rw-   0        0        0     5952 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/schema/sqlite.sql
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.445670 Supysonic-0.7.5/supysonic/server/
--rw-rw-rw-   0        0        0     3395 2023-03-25 14:13:16.000000 Supysonic-0.7.5/supysonic/server/__init__.py
--rw-rw-rw-   0        0        0      259 2021-11-01 14:23:27.000000 Supysonic-0.7.5/supysonic/server/__main__.py
--rw-rw-rw-   0        0        0      828 2023-03-25 14:13:16.000000 Supysonic-0.7.5/supysonic/server/_base.py
--rw-rw-rw-   0        0        0      936 2023-02-11 13:36:47.000000 Supysonic-0.7.5/supysonic/server/gevent.py
--rw-rw-rw-   0        0        0     1289 2023-03-25 14:13:16.000000 Supysonic-0.7.5/supysonic/server/gunicorn.py
--rw-rw-rw-   0        0        0      780 2023-03-25 14:13:16.000000 Supysonic-0.7.5/supysonic/server/waitress.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.375453 Supysonic-0.7.5/supysonic/static/
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.445670 Supysonic-0.7.5/supysonic/static/css/
--rw-rw-rw-   0        0        0    23409 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/css/bootstrap-theme.min.css
--rw-rw-rw-   0        0        0    25648 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/css/bootstrap-theme.min.css.map
--rw-rw-rw-   0        0        0   121200 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   542194 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      794 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/css/supysonic.css
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.455618 Supysonic-0.7.5/supysonic/static/fonts/
--rw-rw-rw-   0        0        0    20127 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   108738 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2021-01-23 14:45:18.000000 Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.455618 Supysonic-0.7.5/supysonic/static/js/
--rw-rw-rw-   0        0        0    37045 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      441 2021-04-10 13:49:54.000000 Supysonic-0.7.5/supysonic/static/js/supysonic.js
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.465554 Supysonic-0.7.5/supysonic/templates/
--rw-rw-rw-   0        0        0     1336 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/addfolder.html
--rw-rw-rw-   0        0        0     2229 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/adduser.html
--rw-rw-rw-   0        0        0     1346 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/change_mail.html
--rw-rw-rw-   0        0        0     2053 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/change_pass.html
--rw-rw-rw-   0        0        0     1179 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/change_username.html
--rw-rw-rw-   0        0        0     2584 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/folders.html
--rw-rw-rw-   0        0        0     2867 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/home.html
--rw-rw-rw-   0        0        0     4204 2021-11-28 14:09:30.000000 Supysonic-0.7.5/supysonic/templates/layout.html
--rw-rw-rw-   0        0        0     1656 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/login.html
--rw-rw-rw-   0        0        0     1478 2021-04-10 13:49:44.000000 Supysonic-0.7.5/supysonic/templates/playlist.html
--rw-rw-rw-   0        0        0      314 2021-04-10 13:49:54.000000 Supysonic-0.7.5/supysonic/templates/playlist_export.m3u
--rw-rw-rw-   0        0        0     4380 2021-04-10 13:49:54.000000 Supysonic-0.7.5/supysonic/templates/playlists.html
--rw-rw-rw-   0        0        0     6598 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/profile.html
--rw-rw-rw-   0        0        0     2378 2021-01-23 14:44:56.000000 Supysonic-0.7.5/supysonic/templates/users.html
--rw-rw-rw-   0        0        0      640 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/utils.py
--rw-rw-rw-   0        0        0     9732 2023-02-11 13:34:27.000000 Supysonic-0.7.5/supysonic/watcher.py
--rw-rw-rw-   0        0        0     2764 2023-03-18 11:40:04.000000 Supysonic-0.7.5/supysonic/web.py
-drwxrwxrwx   0        0        0        0 2023-04-02 14:19:03.465554 Supysonic-0.7.5/tests/
--rw-rw-rw-   0        0        0     3386 2023-02-11 13:34:27.000000 Supysonic-0.7.5/tests/testbase.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:33.236352 Supysonic-0.7.6/
+-rw-rw-rw-   0        0        0    34520 2021-01-23 14:44:54.000000 Supysonic-0.7.6/LICENSE
+-rw-rw-rw-   0        0        0      154 2021-12-19 16:15:13.000000 Supysonic-0.7.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1712 2023-07-14 13:28:31.746615 Supysonic-0.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2738 2023-04-10 13:06:12.000000 Supysonic-0.7.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.676579 Supysonic-0.7.6/Supysonic.egg-info/
+-rw-rw-rw-   0        0        0     1712 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4802 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-12-31 16:33:42.000000 Supysonic-0.7.6/Supysonic.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      108 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3005 2023-04-10 13:06:12.000000 Supysonic-0.7.6/config.sample
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:33.646637 Supysonic-0.7.6/man/
+-rw-rw-rw-   0        0        0     3675 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-cli-folder.1
+-rw-rw-rw-   0        0        0     4128 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-cli-user.1
+-rw-rw-rw-   0        0        0     2769 2023-07-14 13:28:33.566552 Supysonic-0.7.6/man/supysonic-cli.1
+-rw-rw-rw-   0        0        0     1852 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-daemon.1
+-rw-rw-rw-   0        0        0     2984 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-server.1
+-rw-rw-rw-   0        0        0      108 2022-04-23 14:58:53.000000 Supysonic-0.7.6/pyproject.toml
+-rw-rw-rw-   0        0        0     2175 2023-07-14 13:28:31.746615 Supysonic-0.7.6/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-06-18 13:52:50.000000 Supysonic-0.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.686553 Supysonic-0.7.6/supysonic/
+-rw-rw-rw-   0        0        0      534 2023-07-14 13:16:51.000000 Supysonic-0.7.6/supysonic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.686553 Supysonic-0.7.6/supysonic/api/
+-rw-rw-rw-   0        0        0     4059 2023-07-14 10:03:57.000000 Supysonic-0.7.6/supysonic/api/__init__.py
+-rw-rw-rw-   0        0        0     9758 2023-03-18 16:38:26.000000 Supysonic-0.7.6/supysonic/api/albums_songs.py
+-rw-rw-rw-   0        0        0     4941 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/annotation.py
+-rw-rw-rw-   0        0        0     5690 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/api/browse.py
+-rw-rw-rw-   0        0        0      856 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/chat.py
+-rw-rw-rw-   0        0        0     1035 2023-02-25 16:35:07.000000 Supysonic-0.7.6/supysonic/api/errors.py
+-rw-rw-rw-   0        0        0     3585 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/exceptions.py
+-rw-rw-rw-   0        0        0     5165 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/formatters.py
+-rw-rw-rw-   0        0        0     2625 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/jukebox.py
+-rw-rw-rw-   0        0        0    15944 2023-03-18 14:45:11.000000 Supysonic-0.7.6/supysonic/api/media.py
+-rw-rw-rw-   0        0        0     3394 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/playlists.py
+-rw-rw-rw-   0        0        0     1878 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/radio.py
+-rw-rw-rw-   0        0        0     1367 2021-11-28 15:13:37.000000 Supysonic-0.7.6/supysonic/api/scan.py
+-rw-rw-rw-   0        0        0     6948 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/search.py
+-rw-rw-rw-   0        0        0      434 2021-11-28 15:13:37.000000 Supysonic-0.7.6/supysonic/api/system.py
+-rw-rw-rw-   0        0        0      661 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/unsupported.py
+-rw-rw-rw-   0        0        0     2883 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/user.py
+-rw-rw-rw-   0        0        0     7911 2021-01-23 14:44:54.000000 Supysonic-0.7.6/supysonic/cache.py
+-rw-rw-rw-   0        0        0     9784 2023-04-20 14:50:42.000000 Supysonic-0.7.6/supysonic/cli.py
+-rw-rw-rw-   0        0        0     2708 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/config.py
+-rw-rw-rw-   0        0        0     2070 2022-01-30 15:22:37.000000 Supysonic-0.7.6/supysonic/covers.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/daemon/
+-rw-rw-rw-   0        0        0     1668 2023-04-20 15:15:30.000000 Supysonic-0.7.6/supysonic/daemon/__init__.py
+-rw-rw-rw-   0        0        0      259 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/daemon/__main__.py
+-rw-rw-rw-   0        0        0     5313 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/daemon/client.py
+-rw-rw-rw-   0        0        0      252 2021-01-23 14:44:54.000000 Supysonic-0.7.6/supysonic/daemon/exceptions.py
+-rw-rw-rw-   0        0        0     3744 2023-04-20 15:57:38.000000 Supysonic-0.7.6/supysonic/daemon/server.py
+-rw-rw-rw-   0        0        0    20278 2023-05-01 12:09:18.000000 Supysonic-0.7.6/supysonic/db.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/frontend/
+-rw-rw-rw-   0        0        0     2382 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/frontend/__init__.py
+-rw-rw-rw-   0        0        0     2747 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/frontend/folder.py
+-rw-rw-rw-   0        0        0     2627 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/frontend/playlist.py
+-rw-rw-rw-   0        0        0     9366 2023-07-14 10:03:57.000000 Supysonic-0.7.6/supysonic/frontend/user.py
+-rw-rw-rw-   0        0        0     4204 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/jukebox.py
+-rw-rw-rw-   0        0        0     3519 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/lastfm.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/managers/
+-rw-rw-rw-   0        0        0      200 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/managers/__init__.py
+-rw-rw-rw-   0        0        0     2173 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/managers/folder.py
+-rw-rw-rw-   0        0        0     2528 2023-05-01 12:09:18.000000 Supysonic-0.7.6/supysonic/managers/user.py
+-rw-rw-rw-   0        0        0    13097 2023-04-20 15:57:38.000000 Supysonic-0.7.6/supysonic/scanner.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/schema/
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.672073 Supysonic-0.7.6/supysonic/schema/migration/
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.706673 Supysonic-0.7.6/supysonic/schema/migration/mysql/
+-rw-rw-rw-   0        0        0      292 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20161030.sql
+-rw-rw-rw-   0        0        0      227 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20171022.sql
+-rw-rw-rw-   0        0        0     2758 2023-01-08 15:12:52.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20171230.py
+-rw-rw-rw-   0        0        0     3030 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20180221.sql
+-rw-rw-rw-   0        0        0      386 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20180317.sql
+-rw-rw-rw-   0        0        0      208 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20180521.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20181010.sql
+-rw-rw-rw-   0        0        0     1452 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190324.sql
+-rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190518.sql
+-rw-rw-rw-   0        0        0     2767 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190915.sql
+-rw-rw-rw-   0        0        0       73 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190921.sql
+-rw-rw-rw-   0        0        0      266 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20200607.sql
+-rw-rw-rw-   0        0        0     2745 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20230111.py
+-rw-rw-rw-   0        0        0      155 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20230115.sql
+-rw-rw-rw-   0        0        0       88 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20230331.sql
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.706673 Supysonic-0.7.6/supysonic/schema/migration/mysql/__pycache__/
+-rw-rw-rw-   0        0        0     2400 2023-01-11 21:50:42.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.716560 Supysonic-0.7.6/supysonic/schema/migration/postgres/
+-rw-rw-rw-   0        0        0      267 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20161030.sql
+-rw-rw-rw-   0        0        0      232 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20171022.sql
+-rw-rw-rw-   0        0        0      229 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20180311.sql
+-rw-rw-rw-   0        0        0     1136 2023-01-08 15:12:52.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20180317.py
+-rw-rw-rw-   0        0        0      188 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20180521.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20181010.sql
+-rw-rw-rw-   0        0        0     1748 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190324.sql
+-rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190518.sql
+-rw-rw-rw-   0        0        0     3649 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190915.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190921.sql
+-rw-rw-rw-   0        0        0      204 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20200607.sql
+-rw-rw-rw-   0        0        0      153 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20230115.sql
+-rw-rw-rw-   0        0        0       88 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20230331.sql
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.716560 Supysonic-0.7.6/supysonic/schema/migration/sqlite/
+-rw-rw-rw-   0        0        0     1176 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20161030.sql
+-rw-rw-rw-   0        0        0      882 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171022.sql
+-rw-rw-rw-   0        0        0     2032 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171230.py
+-rw-rw-rw-   0        0        0     1629 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180311.sql
+-rw-rw-rw-   0        0        0      939 2023-01-08 15:12:52.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180317.py
+-rw-rw-rw-   0        0        0      754 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180521.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20181010.sql
+-rw-rw-rw-   0        0        0     1746 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190324.sql
+-rw-rw-rw-   0        0        0     1858 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190518.sql
+-rw-rw-rw-   0        0        0     5084 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190915.sql
+-rw-rw-rw-   0        0        0       61 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190921.sql
+-rw-rw-rw-   0        0        0      207 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20200607.sql
+-rw-rw-rw-   0        0        0     1924 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230111.py
+-rw-rw-rw-   0        0        0      499 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230115.sql
+-rw-rw-rw-   0        0        0       87 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230331.sql
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.716560 Supysonic-0.7.6/supysonic/schema/migration/sqlite/__pycache__/
+-rw-rw-rw-   0        0        0     1743 2023-02-11 13:37:00.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6463 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/mysql.sql
+-rw-rw-rw-   0        0        0     5689 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/postgres.sql
+-rw-rw-rw-   0        0        0     5952 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/sqlite.sql
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.726771 Supysonic-0.7.6/supysonic/server/
+-rw-rw-rw-   0        0        0     3395 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/__init__.py
+-rw-rw-rw-   0        0        0      259 2021-11-01 14:23:27.000000 Supysonic-0.7.6/supysonic/server/__main__.py
+-rw-rw-rw-   0        0        0      828 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/_base.py
+-rw-rw-rw-   0        0        0      936 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/server/gevent.py
+-rw-rw-rw-   0        0        0     1289 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/gunicorn.py
+-rw-rw-rw-   0        0        0      780 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/waitress.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.672073 Supysonic-0.7.6/supysonic/static/
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.726771 Supysonic-0.7.6/supysonic/static/css/
+-rw-rw-rw-   0        0        0    23409 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css
+-rw-rw-rw-   0        0        0    25648 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css.map
+-rw-rw-rw-   0        0        0   121200 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   542194 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      794 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/supysonic.css
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.736752 Supysonic-0.7.6/supysonic/static/fonts/
+-rw-rw-rw-   0        0        0    20127 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   108738 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2021-01-23 14:45:18.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.736752 Supysonic-0.7.6/supysonic/static/js/
+-rw-rw-rw-   0        0        0    37045 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      441 2021-04-10 13:49:54.000000 Supysonic-0.7.6/supysonic/static/js/supysonic.js
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.746615 Supysonic-0.7.6/supysonic/templates/
+-rw-rw-rw-   0        0        0     1336 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/addfolder.html
+-rw-rw-rw-   0        0        0     2229 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/adduser.html
+-rw-rw-rw-   0        0        0     1346 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/change_mail.html
+-rw-rw-rw-   0        0        0     2053 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/change_pass.html
+-rw-rw-rw-   0        0        0     1179 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/change_username.html
+-rw-rw-rw-   0        0        0     2584 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/folders.html
+-rw-rw-rw-   0        0        0     2867 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/home.html
+-rw-rw-rw-   0        0        0     4204 2021-11-28 14:09:30.000000 Supysonic-0.7.6/supysonic/templates/layout.html
+-rw-rw-rw-   0        0        0     1656 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/login.html
+-rw-rw-rw-   0        0        0     1478 2021-04-10 13:49:44.000000 Supysonic-0.7.6/supysonic/templates/playlist.html
+-rw-rw-rw-   0        0        0      314 2021-04-10 13:49:54.000000 Supysonic-0.7.6/supysonic/templates/playlist_export.m3u
+-rw-rw-rw-   0        0        0     4380 2021-04-10 13:49:54.000000 Supysonic-0.7.6/supysonic/templates/playlists.html
+-rw-rw-rw-   0        0        0     6598 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/profile.html
+-rw-rw-rw-   0        0        0     2378 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/users.html
+-rw-rw-rw-   0        0        0      640 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/utils.py
+-rw-rw-rw-   0        0        0     9565 2023-04-21 14:53:50.000000 Supysonic-0.7.6/supysonic/watcher.py
+-rw-rw-rw-   0        0        0     3067 2023-04-20 16:15:42.000000 Supysonic-0.7.6/supysonic/web.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.746615 Supysonic-0.7.6/tests/
+-rw-rw-rw-   0        0        0     3386 2023-02-11 13:34:27.000000 Supysonic-0.7.6/tests/testbase.py
```

### Comparing `Supysonic-0.7.5/LICENSE` & `Supysonic-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/PKG-INFO` & `Supysonic-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supysonic
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python implementation of the Subsonic server API
 Home-page: https://supysonic.readthedocs.io
 Download-URL: https://github.com/spl0k/supysonic
 Author: Alban Féron
 Author-email: alban.feron@gmail.com
 License: GNU AGPLv3
 Keywords: subsonic,music,server
```

### Comparing `Supysonic-0.7.5/README.md` & `Supysonic-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/Supysonic.egg-info/PKG-INFO` & `Supysonic-0.7.6/Supysonic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supysonic
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python implementation of the Subsonic server API
 Home-page: https://supysonic.readthedocs.io
 Download-URL: https://github.com/spl0k/supysonic
 Author: Alban Féron
 Author-email: alban.feron@gmail.com
 License: GNU AGPLv3
 Keywords: subsonic,music,server
```

### Comparing `Supysonic-0.7.5/Supysonic.egg-info/SOURCES.txt` & `Supysonic-0.7.6/Supysonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/config.sample` & `Supysonic-0.7.6/config.sample`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/man/supysonic-cli-folder.1` & `Supysonic-0.7.6/man/supysonic-cli-folder.1`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-CLI-FOLDER" "1" "Apr 02, 2023" "0.7.5" "Supysonic"
+.TH "SUPYSONIC-CLI-FOLDER" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
 .SH NAME
 supysonic-cli-folder \- Supysonic folder management commands
 .SH SYNOPSIS
 .sp
 supysonic\-cli folder \fI\-\-help\fP
 .sp
 supysonic\-cli folder \fBlist\fP
```

### Comparing `Supysonic-0.7.5/man/supysonic-cli-user.1` & `Supysonic-0.7.6/man/supysonic-cli-user.1`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-CLI-USER" "1" "Apr 02, 2023" "0.7.5" "Supysonic"
+.TH "SUPYSONIC-CLI-USER" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
 .SH NAME
 supysonic-cli-user \- Supysonic user management commands
 .SH SYNOPSIS
 .sp
 supysonic\-cli user \fI\-\-help\fP
 .sp
 supysonic\-cli user \fBlist\fP
```

### Comparing `Supysonic-0.7.5/man/supysonic-cli.1` & `Supysonic-0.7.6/man/supysonic-cli.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-CLI" "1" "Apr 02, 2023" "0.7.5" "Supysonic"
+.TH "SUPYSONIC-CLI" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
 .SH NAME
 supysonic-cli \- Supysonic management command line interface
 .SH SYNOPSIS
 .sp
 supysonic\-cli \fI\-\-help\fP
 .sp
 supysonic\-cli \fBuser\fP [\fIoptions\fP]
```

### Comparing `Supysonic-0.7.5/man/supysonic-daemon.1` & `Supysonic-0.7.6/man/supysonic-daemon.1`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-DAEMON" "1" "Apr 02, 2023" "0.7.5" "Supysonic"
+.TH "SUPYSONIC-DAEMON" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
 .SH NAME
 supysonic-daemon \- Supysonic background daemon
 .SH SYNOPSIS
 .sp
 supysonic\-daemon
 .SH DESCRIPTION
 .sp
```

### Comparing `Supysonic-0.7.5/man/supysonic-server.1` & `Supysonic-0.7.6/man/supysonic-server.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-SERVER" "1" "Apr 02, 2023" "0.7.5" "Supysonic"
+.TH "SUPYSONIC-SERVER" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
 .SH NAME
 supysonic-server \- Python implementation of the Subsonic server API
 .SH SYNOPSIS
 .sp
 supysonic\-server [\fB\-\-server\fP \fIgevent\fP | \fIgunicorn\fP | \fIwaitress\fP] [\fB\-\-host\fP <\fIhostname\fP>] [\fB\-\-port\fP <\fIport\fP>] [\fB\-\-socket\fP <\fIpath\fP>] [\fB\-\-processes\fP <\fIn\fP>] [\fB\-\-threads\fP <\fIn\fP>]
 .SH DESCRIPTION
 .sp
```

### Comparing `Supysonic-0.7.5/setup.cfg` & `Supysonic-0.7.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/setup.py` & `Supysonic-0.7.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 #
 # Copyright (C) 2013-2021 Alban 'spl0k' Féron
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 import os.path
 
-from distutils import dir_util
+from shutil import rmtree
 from setuptools import setup
 from setuptools.command.sdist import sdist as _sdist
 
 
 class sdist(_sdist):
     def make_release_tree(self, base_dir, files):
         super().make_release_tree(base_dir, files)
 
         man_dir = os.path.join(base_dir, "man")
         doctrees_dir = os.path.join(man_dir, ".doctrees")
         self.spawn(["sphinx-build", "-q", "-b", "man", "docs", man_dir])
-        dir_util.remove_tree(doctrees_dir)
+        rmtree(doctrees_dir)
 
 
 if __name__ == "__main__":
     setup(
         cmdclass={"sdist": sdist},
     )
```

### Comparing `Supysonic-0.7.5/supysonic/__init__.py` & `Supysonic-0.7.6/supysonic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 #
 # Copyright (C) 2013-2018 Alban 'spl0k' Féron
 #                    2017 Óscar García Amor
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 NAME = "Supysonic"
-VERSION = "0.7.5"
+VERSION = "0.7.6"
 DESCRIPTION = "Python implementation of the Subsonic server API"
 AUTHOR = "Alban Féron"
 AUTHOR_EMAIL = "alban.feron@gmail.com"
 URL = "https://supysonic.readthedocs.io/"
 DOWNLOAD_URL = "https://github.com/spl0k/supysonic"
 LICENSE = "GNU AGPLv3"
```

### Comparing `Supysonic-0.7.5/supysonic/api/__init__.py` & `Supysonic-0.7.6/supysonic/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file is part of Supysonic.
 # Supysonic is a Python implementation of the Subsonic server API.
 #
-# Copyright (C) 2013-2022 Alban 'spl0k' Féron
+# Copyright (C) 2013-2023 Alban 'spl0k' Féron
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 API_VERSION = "1.12.0"
 
 import binascii
+import logging
 import uuid
 from flask import request
 from flask import Blueprint
 from peewee import IntegrityError
 
 from ..db import ClientPrefs, Folder
 from ..managers.user import UserManager
 
 from .exceptions import GenericError, Unauthorized, NotFound
 from .formatters import JSONFormatter, JSONPFormatter, XMLFormatter
 
 api = Blueprint("api", __name__)
+logger = logging.getLogger(__name__)
 
 
 def api_routing(endpoint):
     def decorator(func):
         viewendpoint = f"{endpoint}.view"
         api.add_url_rule(endpoint, view_func=func, methods=["GET", "POST"])
         api.add_url_rule(viewendpoint, view_func=func, methods=["GET", "POST"])
@@ -53,28 +55,34 @@
     except ValueError:
         return password
 
 
 @api.before_request
 def authorize():
     if request.authorization:
-        user = UserManager.try_auth(
-            request.authorization.username, request.authorization.password
-        )
+        username = request.authorization.username
+        user = UserManager.try_auth(username, request.authorization.password)
         if user is not None:
             request.user = user
             return
+
+        logger.error(
+            "Failed login attempt for user %s (IP: %s)", username, request.remote_addr
+        )
         raise Unauthorized()
 
     username = request.values["u"]
     password = request.values["p"]
     password = decode_password(password)
 
     user = UserManager.try_auth(username, password)
     if user is None:
+        logger.error(
+            "Failed login attempt for user %s (IP: %s)", username, request.remote_addr
+        )
         raise Unauthorized()
 
     request.user = user
 
 
 @api.before_request
 def get_client_prefs():
```

### Comparing `Supysonic-0.7.5/supysonic/api/albums_songs.py` & `Supysonic-0.7.6/supysonic/api/albums_songs.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/annotation.py` & `Supysonic-0.7.6/supysonic/api/annotation.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/browse.py` & `Supysonic-0.7.6/supysonic/api/browse.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/chat.py` & `Supysonic-0.7.6/supysonic/api/chat.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/errors.py` & `Supysonic-0.7.6/supysonic/api/errors.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/exceptions.py` & `Supysonic-0.7.6/supysonic/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/formatters.py` & `Supysonic-0.7.6/supysonic/api/formatters.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/jukebox.py` & `Supysonic-0.7.6/supysonic/api/jukebox.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/media.py` & `Supysonic-0.7.6/supysonic/api/media.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/playlists.py` & `Supysonic-0.7.6/supysonic/api/playlists.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/radio.py` & `Supysonic-0.7.6/supysonic/api/radio.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/scan.py` & `Supysonic-0.7.6/supysonic/api/scan.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/search.py` & `Supysonic-0.7.6/supysonic/api/search.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/unsupported.py` & `Supysonic-0.7.6/supysonic/api/unsupported.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/api/user.py` & `Supysonic-0.7.6/supysonic/api/user.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/cache.py` & `Supysonic-0.7.6/supysonic/cache.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/cli.py` & `Supysonic-0.7.6/supysonic/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of Supysonic.
 # Supysonic is a Python implementation of the Subsonic server API.
 #
-# Copyright (C) 2013-2022 Alban 'spl0k' Féron
+# Copyright (C) 2013-2023 Alban 'spl0k' Féron
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 import click
 import time
 
 from click.exceptions import ClickException
@@ -360,13 +360,15 @@
     user.save()
     click.echo(f"User '{name}' renamed to '{newname}'")
 
 
 def main():
     config = IniConfig.from_common_locations()
     init_database(config.BASE["database_uri"])
-    cli.main(obj=config)
-    release_database()
+    try:
+        cli.main(obj=config)
+    finally:
+        release_database()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `Supysonic-0.7.5/supysonic/config.py` & `Supysonic-0.7.6/supysonic/config.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/covers.py` & `Supysonic-0.7.6/supysonic/covers.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/daemon/__init__.py` & `Supysonic-0.7.6/supysonic/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/daemon/client.py` & `Supysonic-0.7.6/supysonic/daemon/client.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/daemon/server.py` & `Supysonic-0.7.6/supysonic/daemon/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is part of Supysonic.
 # Supysonic is a Python implementation of the Subsonic server API.
 #
-# Copyright (C) 2019-2022 Alban 'spl0k' Féron
+# Copyright (C) 2019-2023 Alban 'spl0k' Féron
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 import logging
 import time
 
 from multiprocessing.connection import Listener, Client
 from threading import Thread, Event
 
 from .client import DaemonCommand
-from ..db import Folder
+from ..db import Folder, open_connection, close_connection
 from ..jukebox import Jukebox
 from ..scanner import Scanner
 from ..utils import get_secret_key
 from ..watcher import SupysonicWatcher
 
 __all__ = ["Daemon"]
 
@@ -55,30 +55,34 @@
         if self.__config.DAEMON["run_watcher"]:
             self.__watcher = SupysonicWatcher(self.__config)
             self.__watcher.start()
 
         if self.__config.DAEMON["jukebox_command"]:
             self.__jukebox = Jukebox(self.__config.DAEMON["jukebox_command"])
 
+        close_connection()
+
         Thread(target=self.__listen).start()
         while not self.__stopped.is_set():
             time.sleep(1)
 
     def __listen(self):
         while not self.__stopped.is_set():
             conn = self.__listener.accept()
             self.__handle_connection(conn)
 
         self.__listener.close()
 
     def start_scan(self, folders=[], force=False):
         if not folders:
+            open_connection()
             folders = [
                 t[0] for t in Folder.select(Folder.name).where(Folder.root).tuples()
             ]
+            close_connection()
 
         if self.__scanner is not None and self.__scanner.is_alive():
             for f in folders:
                 self.__scanner.queue_folder(f)
             return
 
         extensions = self.__config.BASE["scanner_extensions"]
```

### Comparing `Supysonic-0.7.5/supysonic/db.py` & `Supysonic-0.7.6/supysonic/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,7 +675,15 @@
         version.value = SCHEMA_VERSION
         version.save()
 
 
 def release_database():
     db.close()
     db.initialize(None)
+
+
+def open_connection(reuse=False):
+    return db.connect(reuse)
+
+
+def close_connection():
+    db.close()
```

### Comparing `Supysonic-0.7.5/supysonic/frontend/__init__.py` & `Supysonic-0.7.6/supysonic/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/frontend/folder.py` & `Supysonic-0.7.6/supysonic/frontend/folder.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/frontend/playlist.py` & `Supysonic-0.7.6/supysonic/frontend/playlist.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/frontend/user.py` & `Supysonic-0.7.6/supysonic/frontend/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of Supysonic.
 # Supysonic is a Python implementation of the Subsonic server API.
 #
-# Copyright (C) 2013-2022 Alban 'spl0k' Féron
+# Copyright (C) 2013-2023 Alban 'spl0k' Féron
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 import logging
 
 from flask import flash, redirect, render_template, request, session, url_for
 from flask import current_app
@@ -315,18 +315,22 @@
     if not password:
         flash("Missing password")
         error = True
 
     if not error:
         user = UserManager.try_auth(name, password)
         if user:
+            logger.info("Logged user %s (IP: %s)", name, request.remote_addr)
             session["userid"] = str(user.id)
             flash("Logged in!")
             return redirect(return_url)
         else:
+            logger.error(
+                "Failed login attempt for user %s (IP: %s)", name, request.remote_addr
+            )
             flash("Wrong username or password")
 
     return render_template("login.html")
 
 
 @frontend.route("/user/logout")
 def logout():
```

### Comparing `Supysonic-0.7.5/supysonic/jukebox.py` & `Supysonic-0.7.6/supysonic/jukebox.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/lastfm.py` & `Supysonic-0.7.6/supysonic/lastfm.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/managers/folder.py` & `Supysonic-0.7.6/supysonic/managers/folder.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/managers/user.py` & `Supysonic-0.7.6/supysonic/managers/user.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/scanner.py` & `Supysonic-0.7.6/supysonic/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is part of Supysonic.
 # Supysonic is a Python implementation of the Subsonic server API.
 #
-# Copyright (C) 2013-2022 Alban 'spl0k' Féron
+# Copyright (C) 2013-2023 Alban 'spl0k' Féron
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 import logging
 import os
 import os.path
 import mediafile
 import time
 
 from datetime import datetime
 from queue import Queue, Empty as QueueEmpty
 from threading import Thread, Event
 
 from .covers import find_cover_in_folder, CoverFile
-from .db import Folder, Artist, Album, Track
+from .db import Folder, Artist, Album, Track, open_connection, close_connection
 
 
 logger = logging.getLogger(__name__)
 
 
 class StatsDetails:
     def __init__(self):
@@ -91,14 +91,16 @@
     def queue_folder(self, folder_name):
         if not isinstance(folder_name, str):
             raise TypeError("Expecting string, got " + str(type(folder_name)))
 
         self.__queue.put(folder_name)
 
     def run(self):
+        opened = open_connection(True)
+
         while not self.__stopped.is_set():
             try:
                 folder_name = self.__queue.get(False)
             except QueueEmpty:
                 break
 
             try:
@@ -109,14 +111,17 @@
             self.__scan_folder(folder)
 
         self.prune()
 
         if self.__on_done is not None:
             self.__on_done()
 
+        if opened:
+            close_connection()
+
     def stop(self):
         self.__stopped.set()
 
     def __scan_folder(self, folder):
         logger.info("Scanning folder %s", folder.name)
 
         if self.__on_folder_start is not None:
```

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/mysql/20171230.py` & `Supysonic-0.7.6/supysonic/schema/migration/mysql/20171230.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/mysql/20180221.sql` & `Supysonic-0.7.6/supysonic/schema/migration/mysql/20180221.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/mysql/20190324.sql` & `Supysonic-0.7.6/supysonic/schema/migration/mysql/20190324.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/mysql/20190915.sql` & `Supysonic-0.7.6/supysonic/schema/migration/mysql/20190915.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/mysql/20230111.py` & `Supysonic-0.7.6/supysonic/schema/migration/mysql/20230111.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc` & `Supysonic-0.7.6/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/postgres/20180317.py` & `Supysonic-0.7.6/supysonic/schema/migration/postgres/20180317.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/postgres/20190324.sql` & `Supysonic-0.7.6/supysonic/schema/migration/postgres/20190324.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/postgres/20190915.sql` & `Supysonic-0.7.6/supysonic/schema/migration/postgres/20190915.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20161030.sql` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20161030.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20171022.sql` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171022.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20171230.py` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171230.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20180311.sql` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180311.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20180317.py` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180317.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20180521.sql` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180521.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20190324.sql` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190324.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20190518.sql` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190518.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20190915.sql` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190915.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/20230111.py` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230111.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc` & `Supysonic-0.7.6/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/mysql.sql` & `Supysonic-0.7.6/supysonic/schema/mysql.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/postgres.sql` & `Supysonic-0.7.6/supysonic/schema/postgres.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/schema/sqlite.sql` & `Supysonic-0.7.6/supysonic/schema/sqlite.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/server/__init__.py` & `Supysonic-0.7.6/supysonic/server/__init__.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/server/_base.py` & `Supysonic-0.7.6/supysonic/server/_base.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/server/gevent.py` & `Supysonic-0.7.6/supysonic/server/gevent.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/server/gunicorn.py` & `Supysonic-0.7.6/supysonic/server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/server/waitress.py` & `Supysonic-0.7.6/supysonic/server/waitress.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/css/bootstrap-theme.min.css` & `Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/css/bootstrap-theme.min.css.map` & `Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/css/bootstrap.min.css` & `Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/css/bootstrap.min.css.map` & `Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/css/supysonic.css` & `Supysonic-0.7.6/supysonic/static/css/supysonic.css`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.eot` & `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.svg` & `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.ttf` & `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.woff` & `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/fonts/glyphicons-halflings-regular.woff2` & `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/static/js/bootstrap.min.js` & `Supysonic-0.7.6/supysonic/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/addfolder.html` & `Supysonic-0.7.6/supysonic/templates/addfolder.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/adduser.html` & `Supysonic-0.7.6/supysonic/templates/adduser.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/change_mail.html` & `Supysonic-0.7.6/supysonic/templates/change_mail.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/change_pass.html` & `Supysonic-0.7.6/supysonic/templates/change_pass.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/change_username.html` & `Supysonic-0.7.6/supysonic/templates/change_username.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/folders.html` & `Supysonic-0.7.6/supysonic/templates/folders.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/home.html` & `Supysonic-0.7.6/supysonic/templates/home.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/layout.html` & `Supysonic-0.7.6/supysonic/templates/layout.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/login.html` & `Supysonic-0.7.6/supysonic/templates/login.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/playlist.html` & `Supysonic-0.7.6/supysonic/templates/playlist.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/playlists.html` & `Supysonic-0.7.6/supysonic/templates/playlists.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/profile.html` & `Supysonic-0.7.6/supysonic/templates/profile.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/templates/users.html` & `Supysonic-0.7.6/supysonic/templates/users.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/utils.py` & `Supysonic-0.7.6/supysonic/utils.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.5/supysonic/watcher.py` & `Supysonic-0.7.6/supysonic/watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 
 from threading import Thread, Condition, Timer
 from watchdog.observers import Observer
 from watchdog.events import PatternMatchingEventHandler
 
 from . import covers
-from .db import Folder
+from .db import Folder, open_connection, close_connection
 from .scanner import Scanner
 
 OP_SCAN = 1
 OP_REMOVE = 2
 OP_MOVE = 4
 FLAG_CREATE = 8
 FLAG_COVER = 16
@@ -41,24 +41,17 @@
         except Exception as e:  # pragma: nocover
             logger.critical(e)
 
     def on_created(self, event):
         logger.debug("File created: '%s'", event.src_path)
 
         op = OP_SCAN | FLAG_CREATE
-        if not covers.is_valid_cover(event.src_path):
-            self.queue.put(event.src_path, op)
-
-            dirname = os.path.dirname(event.src_path)
-            try:
-                Folder.get(path=dirname)
-            except Folder.DoesNotExist:
-                self.queue.put(dirname, op | FLAG_COVER)
-        else:
-            self.queue.put(event.src_path, op | FLAG_COVER)
+        if covers.is_valid_cover(event.src_path):
+            op |= FLAG_COVER
+        self.queue.put(event.src_path, op)
 
     def on_deleted(self, event):
         logger.debug("File deleted: '%s'", event.src_path)
 
         op = OP_REMOVE
         _, ext = os.path.splitext(event.src_path)
         if ext in covers.EXTENSIONS:
@@ -150,26 +143,28 @@
             with self.__cond:
                 self.__cond.wait()
 
                 if not self.__queue:
                     continue
 
             logger.debug("Instantiating scanner")
+            open_connection()
             scanner = Scanner()
 
             item = self.__next_item()
             while item:
                 if item.operation & FLAG_COVER:
                     self.__process_cover_item(scanner, item)
                 else:
                     self.__process_regular_item(scanner, item)
 
                 item = self.__next_item()
 
             scanner.prune()
+            close_connection()
             logger.debug("Freeing scanner")
 
     def __process_regular_item(self, scanner, item):
         if item.operation & OP_MOVE:
             logger.info("Moving: '%s' -> '%s'", item.src_path, item.path)
             scanner.move_file(item.src_path, item.path)
```

### Comparing `Supysonic-0.7.5/supysonic/web.py` & `Supysonic-0.7.6/supysonic/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is part of Supysonic.
 # Supysonic is a Python implementation of the Subsonic server API.
 #
-# Copyright (C) 2013-2022 Alban 'spl0k' Féron
+# Copyright (C) 2013-2023 Alban 'spl0k' Féron
 #               2018-2019 Carey 'pR0Ps' Metcalfe
 #                    2017 Óscar García Amor
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 import logging
 import mimetypes
 
 from flask import Flask
 from logging.handlers import TimedRotatingFileHandler
 from os import makedirs, path
 
 from .config import IniConfig
 from .cache import Cache
-from .db import init_database
+from .db import init_database, open_connection, close_connection
 from .utils import get_secret_key
 
 logger = logging.getLogger(__package__)
 
 
 def create_application(config=None):
     global app
@@ -46,14 +46,21 @@
         logger.addHandler(handler)
     loglevel = app.config["WEBAPP"]["log_level"]
     if loglevel:
         logger.setLevel(getattr(logging, loglevel.upper(), logging.NOTSET))
 
     # Initialize database
     init_database(app.config["BASE"]["database_uri"])
+    if not app.testing:
+
+        def open_conn():  # Just to discard the return value
+            open_connection()
+
+        app.before_request(open_conn)
+        app.teardown_request(lambda exc: close_connection())
 
     # Insert unknown mimetypes
     for k, v in app.config["MIMETYPES"].items():
         extension = "." + k.lower()
         if extension not in mimetypes.types_map:
             mimetypes.add_type(v, extension, False)
 
@@ -79,8 +86,11 @@
 
         app.register_blueprint(frontend)
     if app.config["WEBAPP"]["mount_api"]:
         from .api import api
 
         app.register_blueprint(api, url_prefix="/rest")
 
+    if not app.testing:
+        close_connection()
+
     return app
```

### Comparing `Supysonic-0.7.5/tests/testbase.py` & `Supysonic-0.7.6/tests/testbase.py`

 * *Files identical despite different names*

